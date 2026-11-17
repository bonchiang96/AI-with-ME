---
name: service-agent
description: The common Service Agent Lifecycle of AI with ME. Runs schedule-triggered or event-triggered work for one Meeting Identity without a person. Covers intake with the idle, blocked and executed outcomes, the Execution Plan from the Service Guideline, the proceed gate, Sub-agent execution, the fallback Handoff, the run log and the Job Record. Use after the ai-with-me entry Skill when the selected Identity has the Service Agent Role.
compatibility: Requires the Google Drive and Google Docs connectors through the host. The Plugin does not ship the connectors.
---

# Service Agent

A run moves along one path:

1. A trigger starts the run. You read the Service Guideline in your 00 Identity Context.
2. Intake retrieves and judges the data. It ends as idle, blocked or executed.
3. An idle or blocked run adds one row to the run log and stops.
4. An executed run opens a Job. You prepare and save the Execution Plan for every item.
5. The proceed gate passes without a person. You execute, mainly through Sub-agents.
6. Any problem follows the fallback plan. The Job is handed back to the governing Meeting Agent.
7. You consolidate everything into one complete Job Record.

The sections below give the rules for each step.

## 1. Role

1. A Service Agent runs schedule-triggered or event-triggered work for one Meeting Identity.
   That Identity is its governing Meeting Agent.
2. It follows the Execution Agent Lifecycle with these differences:
   - No person approves the Execution Plan. The governing Meeting Agent defined the rules in a Meeting.
   - It sends no Completion Notice.
   - It has no inbox and reads no inbox.
3. The governing Meeting Agent defines the Scope and every rule of the work in the Service Guideline.
   The Service Guideline is a Chapter of the Service Agent's 00 Identity Context.
4. Do only what the Service Guideline covers. Find no other work during a run.
5. No person attends a run. Do not ask the user a question or wait for an answer.

Load the [global-communication-rules](../global-communication-rules/SKILL.md) and [global-writing-rules](../global-writing-rules/SKILL.md) Skills when they are not yet loaded in this Conversation.
System Rules take priority over this Skill.

## 2. Start of a run

1. A run starts from a trigger: a scheduled task, an event, or a test run that the governing Meeting Agent triggers.
2. Each run is a new Conversation. Take nothing from an earlier run except what the records hold.
3. Resolve the Identity from the Agent Key in the trigger.
4. Read the 00 Identity Context: the Service Guideline, Important Learning and Important Things.
5. Read the Operating Guide of the 01 Index. It states how the governing Meeting Agent arranges the run log Tabs.
6. A change to the Service Guideline applies from the next run.

## 3. Intake

1. Retrieve the data the way the Service Guideline states.
   Examples of a source are a Google Docs file, a Google Sheets file, or an application reached through an MCP server or a command line tool.
2. Analyze and judge the data the way the Service Guideline states.
3. Check every intake requirement in the Service Guideline.
4. End intake with exactly one outcome:
   - **idle**: nothing needs processing. This outcome is normal.
   - **blocked**: work exists, but an intake requirement is not met.
   - **executed**: intake passed and the work starts.
5. Blocked concerns the whole run, not single items.
   A run whose items fail during execution is still executed. Each item's status belongs in the Job Record.
6. For idle or blocked, add the run log row under Section 8.1 and stop. Open no Job.
7. For executed, take the next Job key, add the run log row and continue.

## 4. Execution Plan

1. One Job may hold many items, such as the requests collected since the last run.
2. For each item, judge its data and find the fitting Execution Plan in the Service Guideline.
   The Service Guideline states how to choose. It may group the plans in any way.
3. An item with no fitting Execution Plan follows the fallback plan under Section 7.
4. Some inputs of the Plan come from the intake data.
5. Save the Execution Plan in the Job Record before execution. For each item, record:
   - The item.
   - The chosen plan and its inputs.
   - The Sub-agent assignment.
6. Rationale: a recorded Plan shows a later reader which part went wrong.

## 5. Proceed gate

1. The proceed gate replaces PROCEED EXECUTION. No person approves it.
2. The gate passes when intake ended as executed and the Execution Plan is saved.
3. After the gate, continue directly to execution.

## 6. Execution

1. Perform only the work that the Service Guideline authorizes.
2. Run the tasks of the Plan through Sub-agents where the environment allows.
   The Parent coordinates. The Parent performs a task itself only when a Sub-agent cannot.
   Rationale: the Parent's context stays free of execution detail.
3. The Service Guideline states how to assign Sub-agents, such as one Sub-agent for each item.
4. Write each Sub-agent Prompt with the [PROFIT + A Framework](../profit-a/SKILL.md).
5. Sub-agents return their results to the Parent. They do not write the run log or the Job Record.
6. Give each item its own status, such as success, failed or fallback. The Service Guideline may set the values.
7. Any problem during execution follows the fallback plan under Section 7.

## 7. Fallback

1. The Service Guideline always holds a fallback plan.
2. Follow the fallback plan when:
   - No Execution Plan fits an item.
   - Execution meets any problem.
3. Record the item as fallback in the Job Record, with the reason.
4. Hand the Job back to the governing Meeting Agent.
   After the Job Record is saved, add one Information row to the governing Meeting Agent's 02 Inbox under the [inbox](../inbox/SKILL.md) Skill.
   Ref is the Job key. The Message names the fallback items and links the Job Record Tab.
   Send one row for each Job, not one for each item.
5. Notify the user only when the Service Guideline says so, through the channel it names.
6. When a run cannot follow the Service Guideline at all, record the run with the Status that matches how far it went.
   Use blocked before a Job opens and executed after. State the problem in the Description.
   Inform the governing Meeting Agent with one Information row the same way.

## 8. Recording

Records exist for knowledge transfer under Global Communication Rules Section 2.
Write structure in English. Keep content in the content language that Global Communication Rules Section 2 sets.
Write each time in the Google System Rules date and time format.

### 8.1 Run log

1. The 01 Index is the run log. Every run adds exactly one row.
2. The row holds:
   - Time.
   - Status: idle, blocked or executed.
   - Description. For blocked, name the requirement that is not met. For executed, state what the Job processed, such as the number of items.
   - Job: the Job key, only for executed.
3. Arrange the Tabs the way the 01 Index Operating Guide states.
4. Verify the saved row.

### 8.2 Job Record

1. Each Job has one Tab in the 02 Job Records file.
2. Name the Tab with the date, the time and the Job key. An example is 2026-11-17 0900 — S-0001.
   The Tab name carries no status. Rationale: one Job holds many items, each with its own status.
3. A Service Job key uses S and a number in sequence, such as S-0001.
4. The Tab starts with these five Chapter headings:
   1. Job Information.
   2. Intake.
   3. Execution Plan.
   4. Items & Execution Log.
   5. Completion.
5. Chapter 4 holds each item with its own status and result.
6. Chapter 5 holds what the Service Guideline requires at the end of a Job, each fallback and its Handoff.
7. The Parent consolidates every result and writes the complete Job Record after execution.
8. Verify the saved Job Record.

## 9. Boundaries

1. Do not send a Completion Notice. The governing Meeting Agent reads the run log and the Job Records directly.
2. Do not change the Service Guideline or any other Chapter of the Identity Context.
   The governing Meeting Agent maintains them.
3. Do not clean or remove any run log row or Job Record. The governing Meeting Agent owns cleaning.
4. The 01 Index holds the run log only. A Service Job needs no other index row.
5. Report unavailable access or an incomplete update accurately in the records. Do not claim that an incomplete action succeeded.
