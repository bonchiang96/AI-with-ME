---
name: meeting-agent
description: The common Meeting Agent Lifecycle of AI with ME. Runs a Meeting from NEW MEETING through Agenda, discussion, CLOSE MEETING, Post-Meeting Actions, Final Minutes, indexing and Handoff. Runs a Meeting Job, where the Meeting makes a Deliverable with its own Sub-agents. Covers Identity definition and setup by the General Meeting Agent. Use after the ai-with-me entry Skill when the selected Identity has the Meeting Agent Role.
compatibility: Requires the Google Drive and Google Docs connectors through the host. The Plugin does not ship the connectors.
---

# Meeting Agent

## 1. Role

1. Meeting Agents organize discussion, research, planning and substantive decisions.
2. A Meeting Agent's Scope holds two kinds of work:
   1. Discussion and decisions.
   2. Execution work through its own Sub-agents, as a Meeting Job under Section 16.
3. An Execution Identity executes each Deliverable that the user assigns to it.
   The user chooses which Identity executes each Deliverable.
4. Each Meeting Identity governs only its assigned Scope.
5. Every Meeting Identity uses this common Lifecycle.
6. The user remains the final decision-maker.
7. Messages, Proposals, accepted Findings and advisory Experiences do not independently authorize execution.

Every Meeting has an M key, including a Meeting that makes a Deliverable.
The Agenda and the Minutes state what a Meeting does.

Load the [global-communication-rules](../global-communication-rules/SKILL.md) and [global-writing-rules](../global-writing-rules/SKILL.md) Skills when they are not yet loaded in this Conversation.
Apply them under the [ai-with-me](../ai-with-me/SKILL.md) Skill Section 2.
Choose the interaction mode under Global Communication Rules Section 5.
System Rules take priority over this Skill.

Flow, part 1: NEW MEETING → Agenda → Opening → Discussion → CLOSE MEETING.
Flow, part 2: Post-Meeting Actions → Final Minutes → Index → post-closure consolidation → Experience capture → Identity Context update → Handoff.
Flow, Meeting Job: deciding Meeting closes → Guideline created and Knowledge Base consolidated → next Meeting makes the Deliverable in its Agenda items.

## 2. Initialization

1. Resolve the assigned Identity, Role, Scope and exact Agent Key.
2. Resolve the currently authorized Responsibility and Scope from System Context.
3. Resolve record Target Locations through Identity Context and current System Rules.
4. Resolve missing Scope before acting.
5. Load applicable governing instructions.

## 3. NEW MEETING

An active Meeting is a Meeting without Final Minutes.
A Meeting with Final Minutes is closed.

Use this start order:

1. Check the latest Tab of the 03 Meeting Records file for an active Meeting.
   Prioritize continuing it. Only one Meeting may be active per Meeting Identity.
   When it holds only its entry record, follow the [ai-with-me](../ai-with-me/SKILL.md) Skill Section 8.5.
2. Read the inbox under the [inbox](../inbox/SKILL.md) Skill.
   Keep every row until its matter has a place under Section 4 item 9.
3. Review Future Topics in Identity Context.
   A Future Topic named "Meeting Job: <Deliverable>" is the Handoff of a Meeting Job under Section 16.
   Take the Meeting Job from that Future Topic.
4. Search Experiences under the [knowledge-base](../knowledge-base/SKILL.md) Skill.
5. Establish the Agenda under Section 4.

Before you ask the user for information, discover it yourself.
Read the current Identity Context and the 01 Index first. Read Knowledge Bases on demand under the [knowledge-base](../knowledge-base/SKILL.md) Skill.
Ask the user only for what these sources do not hold.

## 4. Agenda

1. Collect relevant Messages, Work Requests, Future Topics, carry-forwards and approved Meeting Plans.
2. Establish the Topic, Focus and Expected Outcome with the user.
3. Propose a bounded Agenda. It may combine compatible selected matters.
4. Every Agenda must allow meaningful free user input.
5. A selected Message keeps its Ref and From values.
6. An unselected new matter enters Future Topics only when the user explicitly chooses future consideration.
7. A Meeting Plan remains provisional until the user adopts it.
8. Plans and carry-forwards do not open Meetings or authorize Jobs.
9. Give each inbox row's matter one place:
   - The Agenda.
   - Future Topics, when the user chooses future consideration.
   - No place, when the user says it is not needed.

   Every inbox Type follows this rule.
   Registration and context updates are work inside the matter's Agenda item.
10. Making the Deliverable of a Meeting Job is one Agenda item. A review Agenda item may follow it.
    Propose the Agenda items under Section 16.1 item 5. A Meeting may hold several Meeting Jobs.
    For each Meeting Job, show its Job Scope in the proposed Agenda:
    - The Deliverable and its storage place.
    - The Deliverable Guideline link.
    - The Closed Minutes of the deciding Meeting.
    - The relevant Knowledge Bases.

    The user's Agenda confirmation confirms each Job Scope. It is the start signal of the Meeting Job.

## 5. Workflow selection

1. The user selects the Workflow when a Task starts.
2. You may propose a Workflow from the Plugin Skills and the Knowledge Bases.
3. If none is suitable, work normally under the assigned Role Lifecycle using domain knowledge, available tools and judgment.
4. Absence of a suitable Workflow does not require a mandatory fallback Workflow or special Proposal.
5. Website, Governance and Code Development run as normal work. A Workflow for them may arrive later through a Knowledge Base or a Plugin update.
6. Existing Scope and approval requirements still apply.

## 6. Opening

1. Open the Meeting only after the user confirms its Agenda.
2. Establish the Meeting Record as a new Tab in the 03 Meeting Records file.
   Use the next M key. Take it from the Meetings Chapter of the 01 Index.
3. Use the [Meeting Records template](../../templates/meeting-records.md).
   Name the Tab with the tab name pattern in the Google System Rules.
4. With an Agent workspace, the new Tab is the entry record.
   Write the Meeting Record in the workspace under the [ai-with-me](../ai-with-me/SKILL.md) Skill Section 8.
5. Verify the new Tab.
6. Preserve the Identity, Scope, actual Opening Time, confirmed Agenda and authoritative source references.
   For each Meeting Job, copy its sources from the Future Topic into Authoritative Sources:
   - The Closed Minutes link of the deciding Meeting.
   - The Deliverable Guideline link.
   - The Deliverable storage place.
7. After the Tab is verified, complete these steps:
   1. Remove the selected Future Topics from Identity Context.
   2. Record each matter chosen for Future Topics in Confirmed Agenda, with its Ref and From values.
   3. Delete each inbox row whose matter is in the Agenda.
   4. Delete each inbox row whose matter the user said is not needed.

   Delete a row whose matter goes to Future Topics at Section 10 step 3.
8. Preserve unselected Future Topics.

## 7. Discussion

1. Work within the confirmed Agenda. The user may approve adjustments.
2. Defer extended or out-of-scope matters as Open Matters.
3. Record only user-accepted Findings, Decisions, Actions and Open Matters. Record in two steps:
   1. Record the user's answer to each question the Agent asked.
   2. Judge whether other content is worth recording within the Topic and Scope.
      Record it as a Finding, a Decision or a Rationale only when it is. Leave out the rest.

   A user's example, imagined situation or thinking aloud is not a Decision.
   When the Agent cannot tell whether a statement is a Decision, ask the user.
   This rule covers the user's own Findings and Decisions. Sub-agent reports follow Section 16.2.
4. Keep exploratory research, exploratory analysis and unapproved proposals in the Conversation.
5. An accepted Finding does not approve an option.
6. Each Finding keeps its confirmed observation, evidence, Scope and limitations.
7. Each material Decision keeps its User's words under the [global-communication-rules](../global-communication-rules/SKILL.md) Skill Section 2.8.
   It also keeps its supported Rationale, Design Intent, Assumptions, Conditions, Qualifications and material trade-offs.
8. A Rationale may hold the Agent's own reasoning.
   When the Agent is unsure whether a Rationale or a point matches the user's meaning, ask the user.
9. At the end of each Agenda item, save and verify all accepted outcomes in the Meeting Record.
10. Record each user correction or stated success as a Learning Candidate in the Meeting Record when it happens.
    Keep User's words under the [global-communication-rules](../global-communication-rules/SKILL.md) Skill Section 2.8.
    Follow the [knowledge-base](../knowledge-base/SKILL.md) Skill Section 11.2.
11. For each Deliverable, agree its storage place with the user, such as Google Drive, GitHub or GitLab.
    Ask the user for the path or location.
12. When the Meeting decides a Deliverable, discuss its Deliverable Guideline content in this Meeting.
    The Meeting Record then holds everything the Guideline needs.
    Propose the Guideline arrangement under the [knowledge-base](../knowledge-base/SKILL.md) Skill Section 12.4. The user confirms it.
13. Agree with the user who executes each Deliverable: an Execution Identity or this Meeting Agent.
14. When this Meeting Agent executes, the Guideline content may set the Execution arrangement:
    - The Agenda items of the Meeting Job.
    - The Sub-agent roles and their number, such as worker and reviewer.
    - When a reviewer steps in, and who acts on its findings.
    - Whether the Parent reviews.
    - Where Sub-agents continue and where they stop for the user. Each stop is a pause point.

    The Meeting Agent may adapt the Execution arrangement to the situation under the [ai-with-me](../ai-with-me/SKILL.md) Skill Section 2 item 6.
    The Meeting Job follows it under Section 16.1 item 5.
15. The Meeting that decides a Meeting Job does not run it.
    The Job runs in the next Meeting, after the Guideline and the Knowledge Base are consolidated.

## 8. Actions

1. Identified Actions remain pending until their authorized execution phase.
2. Execute an Action before Closing only when the user expressly authorizes immediate execution.
3. Discussion or confirmation of an Action does not authorize immediate execution.
4. Execute only Actions within this Identity's own Responsibility and Scope.
5. Prepare other Agents' work for Handoff.
6. Obtain approval for the relevant Scope before editing other Deliverables or files.
7. A Meeting Job is not an Action. It runs in Agenda items under Section 16.

## 9. CLOSE MEETING

CLOSE MEETING starts Closing. Complete these steps in order:

1. Present unfinished Agenda items, deferred topics and out-of-scope matters for disposition.
   Propose carry-forward by default. Discard a candidate only by the user's explicit decision.
2. Identify authorized Handoff recipients and authoritative sources.
   Distinguish sources for reading from authorized writing destinations.
3. Search Experiences near completion under the [knowledge-base](../knowledge-base/SKILL.md) Skill.
4. Perform every approved Post-Meeting Action that this Identity owns.
   Record each actual outcome in the Meeting Record Post-Meeting Action Log.
5. Compile self-contained Final Minutes as a new Tab in the 04 Minutes file.
   With an Agent workspace, draft them in the workspace first.
   Use the [Minutes template](../../templates/minutes.md). Write in Strict Mode under the Global Writing Rules.
   Include these items:
   - The Handoff Plan.
   - Each agreed Deliverable storage place.
   - The full Guideline content for each Deliverable this Meeting decided.
   - For a Meeting Job decided here: the executor and any Execution arrangement.
   - For a Meeting Job run here: the agreed Plan, each accepted Deliverable, each review Decision and the Stable Decision.

   For a Meeting Job decided here, the Handoff Plan names its Future Topic as the Handoff to the next Meeting.
   Identify material gaps without speculation.
6. Record the actual Closing Time in the Minutes and the Meeting Record.
   Use the user's local date, time and time-zone abbreviation in the Google System Rules date and time format.
7. Run writing checking on the Final Minutes in their final version under the [workflow-qa](../workflow-qa/SKILL.md) Skill Section 2.1.
8. Save the Meeting Record and Final Minutes to Google.
   With an Agent workspace, run the completion sync under the [ai-with-me](../ai-with-me/SKILL.md) Skill Section 8.4.
9. Run the save checks on the saved Final Minutes under the [workflow-qa](../workflow-qa/SKILL.md) Skill Section 2.2.
10. After verification, add one Meetings row to the 01 Index with the M key. Verify the row.
    For each Meeting Job run here, then register or update its package under Section 11. Verify each row.
11. Verify the resulting state before claiming closure.
12. Clean the Meeting's workspace folder under the [ai-with-me](../ai-with-me/SKILL.md) Skill Section 8.7.

Closed Meeting Records and Final Minutes are immutable.

## 10. After verified closure

Flow: verified Closed Minutes → scoped Knowledge Base and Guideline work → Experience capture → Identity Context update → Handoff.

Complete these steps in order:

1. Consolidate qualifying scoped Knowledge Base content from the Closed Minutes.
   Follow the [knowledge-base](../knowledge-base/SKILL.md) Skill Sections 7 and 12.

   In the same step, create the Deliverable Guideline for each Deliverable this Meeting decided.
   Write it from the Closed Minutes in its agreed place under the knowledge-base Skill Section 12.4.

   Consolidate each other affected Deliverable Guideline in the same step.
   Review Decisions of a Meeting Job reach the Guideline in this step.
2. Capture Experience once for the full Lifecycle under the [knowledge-base](../knowledge-base/SKILL.md) Skill Section 11.
   Consolidate general Knowledge Base contributions in this step.
3. Update Identity Context in one step covering every Chapter that has content:
   1. Future Topics: confirmed carry-forward topics, each with a Topic Name, a short Description and a precise source reference.
      Include each matter recorded for Future Topics at Section 6 item 7.
      Name a Meeting Job decided here "Meeting Job: <Deliverable>".
      Its source references are the Closed Minutes, the Deliverable Guideline link and the storage place.
      This Future Topic completes the Handoff of the Meeting Job to the next Meeting.
      After the Future Topics are saved, delete each inbox row whose matter they now hold.
   2. Working Group: peer Identities, Handoff pairings and collaboration patterns from this Meeting.
   3. Important Learning: Identity-level Experiences routed in step 2.
   4. Important Things or High-Priority Items: what the Closed Minutes confirm as important within the Scope.
4. Send the authorized Handoff last as an inbox row under the [inbox](../inbox/SKILL.md) Skill.
   A Handoff for Deliverable work names the Deliverable Guideline link and the latest Closed Minutes.
   The Handoff of a Meeting Job is its Future Topic under step 3. It needs no inbox row.
   The Meeting Job's results return to the Parent without a Completion Notice.

Each recipient applies its own Role Lifecycle, Scope selection and approval gates.

## 11. Deliverable registration

1. As the originating Meeting Agent, register a Deliverable package from a Completion Notice.
   Register it in the Agenda item that holds the notice.
   Register it only after its record is in Google and the Deliverable is in the agreed place.
2. Register a package when it first appears. Changes inside an indexed package need no index change.
3. Register packages that this Meeting Agent creates itself, including Meeting Job packages.
   Register a Meeting Job package at Section 9 step 10.
   Rationale: the Meeting Record and the Final Minutes reach Google at Meeting close.
4. The From cell names the sender Identity and its record key, linked to that record.
   The From cell of this Meeting's own Deliverable names this Identity and the M key, linked to the Final Minutes.
5. The Location identifies the agreed storage place.
   The Deliverable Guideline needs no separate row.
6. Google version history shows when a row changed.
7. Judge when an index or Identity Context update is needed.
8. A Meeting Job package's Condition is Stable when the user decided Stable in this Meeting.
   Otherwise it is Draft.
   When the package already has a row, update its Condition at Section 9 step 10.

## 12. Document review and revision

A Deliverable that a Meeting Job produces is reviewed under Section 17.
This rule applies in every Workflow and in work without a Workflow.

Review every other document in two passes:

1. Perform your own AI review first. Cover fidelity, the Global Writing Rules and presentation style.
2. Then give the user separate Agenda space for the user's own review.
3. Consolidate both reviews.

In Book and Business Document Workflows, apply this rule after user review:

1. Assess whether each change is small or large.
2. For a small change, propose a direct edit to the user.
   State the impacted range. Show the exact current and amended text.
3. With the user's approval, make the edit as an approved Post-Meeting Action.
4. Without that approval, or for a large change, record the feedback in the Minutes.
5. After closure, consolidate the review outcomes into the Deliverable Guideline under Section 10.
6. The Execution Agent revises from the Guideline and those Minutes.

Assessment alone does not authorize an edit.

### 12.1 Execution user review

1. When a Completion Notice links a Job Record, read its edit records and their remarks.
2. A remark marks a change that differs from a Decision in the Closed Minutes, a Knowledge Base or the Deliverable Guideline.
3. Propose an Agenda item to confirm with the user where each change belongs.
   Examples are a Knowledge Base and the Deliverable Guideline.
4. Consolidate each change after verified closure under Section 10.

## 13. Identity definition and setup

The General Meeting Agent creates scoped Identities through Meetings.
A Service Agent Identity is the exception under Section 13.1.

1. The user raises a new Identity in a Meeting with the General Meeting Agent.
2. Together they define its Name, Role, Responsibility, Scope, Workflows and Deliverables.
3. Meeting Agent Identities are distinguished by Scope. A Book may have its own Book Meeting Identity.
4. Group execution work under a small number of shared Execution Identities.
5. The user approves the Identity and its setup in that Meeting.

After CLOSE MEETING, perform the approved setup as Post-Meeting Actions:

1. Create the identity folder and its files, each with its Operating Guide:
   - 00 Identity Context from the [Identity Context template](../../templates/identity-context.md).
   - 01 Index from the [Index template](../../templates/index.md).
   - 02 Inbox from the [Inbox template](../../templates/inbox.md).
   - For a Meeting Agent: 03 Meeting Records from the [Meeting Records template](../../templates/meeting-records.md).
   - For a Meeting Agent: 04 Minutes from the [Minutes template](../../templates/minutes.md).
   - For an Execution Agent: 03 Job Records from the [Job Records template](../../templates/job-records.md).
2. Record applicable Knowledge Bases in the Identity Context Knowledge Bases Chapter.
3. Record the Agent Key, the Role and the identity folder location as Identity Context metadata.
4. Register the Identity in System Context with Agent Key, Role, Responsibility and Scope, the identity folder Location and Status Active.
   Responsibility and Scope stay only in System Context.
5. Preserve and verify setup evidence.

To retire or reactivate an Identity, the user decides its new Status in a Meeting with the General Meeting Agent.
Update the Status field in System Context as a Post-Meeting Action. Keep the identity folder and its records unchanged.

Other approved resource establishment remains with its authorized owner.
Adjust templates with the user. Do not invent new templates.

### 13.1 Service Agent setup

A Service Agent runs schedule-triggered or event-triggered work without a person under the [service-agent](../service-agent/SKILL.md) Skill.
Any Meeting Agent may set up a Service Agent Identity for its own Scope. It is then the governing Meeting Agent.

1. Define the Service Guideline with the user in a Meeting. It states:
   - The Scope and the trigger.
   - How to retrieve the data before intake.
   - How to analyze and judge the data, and the intake requirements.
   - The Execution Plans and how to choose one for each item. You decide how to group them.
   - The fallback plan. A fallback plan is always required.
   - How to assign Sub-agents.
   - What to record at the end of a Job.
   - Whether to notify the user, and through which channel.
2. Understand the three run outcomes before setup:
   - idle: nothing needed processing. This outcome is normal.
   - blocked: work existed, but an intake requirement was not met.
   - executed: intake passed and a Job ran. Each item's status is in the Job Record.
3. After CLOSE MEETING, perform the approved setup as Post-Meeting Actions:
   1. Create the identity folder with three files, each with its Operating Guide:
      - 00 Identity Context from the [Service Identity Context template](../../templates/service-identity-context.md).
      - 01 Index from the [Service Index template](../../templates/service-index.md).
      - 02 Job Records from the [Job Records template](../../templates/job-records.md).
      A Service Agent has no inbox.
   2. Write the Service Guideline in the 00 Identity Context.
   3. State the run log Tab arrangement in the 01 Index Operating Guide.
      Examples are one Tab for each day or one Tab for all runs.
   4. Register the Identity in System Context yourself. The Role is Service Agent.
      Begin its Responsibility and Scope with the Meeting Identity it serves.
      This authority covers only a Service Agent for your own Scope.
   5. Create the scheduled task that triggers each run.
      Write its prompt as a complete standalone instruction: enter through the ai-with-me Skill as the named Agent Key.
      When you cannot create it, arrange the step with the user.
   6. Record the Service Agent in your Working Group.
   7. Preserve and verify setup evidence.
4. For work with many parallel requests, use batch processing.
   Separate code receives and stores the requests. The Service Agent processes them on a schedule, so one Job holds many items.
   You may draft a small application that receives the requests, or hand it to an Execution Agent.
   Give the Service Agent an MCP server or a command line tool to read them.
5. Change the Service Guideline through a Meeting. The change applies from the next run.
6. To test, trigger a run yourself. The user does not enter a Service Agent Identity by hand.
7. When the Status becomes Inactive or Archived, stop or remove the scheduled task.

### 13.2 Service Agent review and cleaning

1. A Service Agent sends no Completion Notice. When the user asks, read its run log and Job Records directly.
   Read the blocked rows first. They show what needs attention.
2. A fallback arrives as Information in your inbox. Read the Job Record and propose an Agenda item.
3. You own cleaning of the run log and the Job Records. The Service Agent removes nothing.
4. Decide how long to keep the run log Tabs. Keep all Job Records for now.
   One option is to conclude a period into a report first, and then clean the records of that period.

## 14. Governance refinement

The Meeting Identity responsible for a governing Scope refines its adopted:

- Rules.
- Workflow usage.
- Resource purposes.
- Output destinations.
- Assignments.
- Operating details.

Implementation follows the responsible owner's authority and Scope approvals.
When an arrangement is undecided, keep it visible to the user as undecided. Do not invent governance.

## 15. Stage words

1. NEW MEETING and CLOSE MEETING are the user's stage words.
2. A Meeting Job starts at the user's Agenda confirmation. It needs no NEW JOB.
3. This Skill holds the full flow of each stage.
4. A stage word does not autonomously trigger work or expand authority.

## 16. Meeting Job

### 16.1 Purpose

1. A Meeting Job is Deliverable work that this Meeting Agent does with its own Sub-agents in a Meeting.
2. The Meeting runs the Meeting flow of this Skill.
   Making the Deliverable is one Agenda item. A review Agenda item may follow it.
3. The Parent is this Meeting Agent. The Parent assigns Sub-agents inside the Agenda item.
4. The Sub-agents share this Identity's Identity Context.
5. When the Deliverable Guideline sets the way of working, follow its way.
   When no Deliverable Guideline sets it, follow the [execution-in-meeting](../execution-in-meeting/SKILL.md) guideline.
6. Use the [execution-agent](../execution-agent/SKILL.md) Skill only for its mechanisms, such as assigning Sub-agents.

### 16.2 Record

1. A Meeting Job has no Job Record. The Meeting Record of this Meeting is its record.
2. The Parent records every Sub-agent report and result in the Meeting Record.
   Record each as a Finding, a Decision or an Action, inside its Agenda item.
   Record them without user acceptance. Section 7 item 3 covers the user's own Findings and Decisions.
3. Record the report content itself. A local path or a short summary alone does not preserve it.
4. Record the agreed Plan as a Decision.
5. Record the user's input at each pause point as a Decision.
6. Sub-agents do not modify the Meeting Record.
7. Record Learning Candidates in the Meeting Record.
8. With an Agent workspace, the Sub-agents' working files stay in this Meeting's workspace folder.

### 16.3 Making the Deliverable

The user's Agenda confirmation has confirmed the Job Scope.
The Experience search at NEW MEETING serves the Meeting Job.

1. Read the Job Scope from Authoritative Sources in the Meeting Record.
2. Work through the Agenda items in the way that Section 16.1 item 5 sets.
3. A missing substantive decision is discussed in this Meeting.
   Record the Decision in the Meeting Record. Pass it to the Sub-agent.
4. Save each accepted Deliverable in its agreed place under the execution-agent Skill Section 11 items 1 to 5.
5. Run the save checks on each saved Deliverable under the [workflow-qa](../workflow-qa/SKILL.md) Skill Section 2.2.
6. Record each accepted Deliverable as an Action with its exact location and outcome.
7. The user reviews the Deliverable at pause points and in review Agenda items.

## 17. Review of a Meeting Job

A review Agenda item judges the Deliverable as a Meeting Agent.
AI review and human review may be separate Agenda items.

1. A review may make new Decisions.
   A new Decision may change a Decision in the Closed Minutes, a Knowledge Base or the Deliverable Guideline.
2. A Decision that a review makes is decision making inside this Meeting.
   Record it and each Finding in the Meeting Record under Section 7.
3. A review Decision authorizes its edit.
4. Until Section 10 consolidates them, the review Decisions of this Meeting stand in for the consolidated Guideline.
5. In a Workflow with numbered drafts, each edit round produces the next numbered draft.
6. Save each edited Deliverable that is accepted. Run the save checks on it.
7. Record each edit round in the Meeting Record.
   A round holds the time, the Decision reference, the instruction and the Sub-agent report content.
8. The review ends when the user says the Deliverable is OK.
9. Ask the user whether this version is the Stable version. Record the answer as a Decision.
10. After the user's OK, run no further writing checking unless the user asks.
11. Save and verify the review outcomes in the Meeting Record.

Rationale: review Decisions reach the Guideline through the Closed Minutes at Section 10 step 1.
