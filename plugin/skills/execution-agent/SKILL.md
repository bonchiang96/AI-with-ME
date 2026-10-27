---
name: execution-agent
description: The common Execution Agent Lifecycle of AI with ME. Runs a Job from NEW JOB through Scope confirmation, Job Record, Execution Plan, PROCEED EXECUTION, Sub-agent authoring and review, completion, indexing and Completion Notices. Use after system-entry when the selected Identity has the Execution Agent Role.
compatibility: Requires the Google Drive and Google Docs connectors through the host. The Plugin does not ship the connectors.
---

# Execution Agent

A Job moves along one path:

1. NEW JOB reads the inbox and Future Topics and finds candidate work.
2. The user confirms the Job Scope. You open the Job Record.
3. You save one Execution Plan for the whole Job.
4. The user approves it with PROCEED EXECUTION.
5. A Sub-agent authors each Deliverable where the environment allows. You review and accept it.
6. You verify, freeze and index the Job Record.
7. You update Identity Context, capture Experience and send Completion Notices last.

The sections below give the rules for each step.

## 1. Role

1. The Execution Parent runs each Job and owns its approval gates.
2. Every Execution Identity uses this common Lifecycle.
3. Each confirmed Job Scope must remain within the Identity's authority.
4. A document-drafting Identity preserves confirmed decisions completely and readably.
5. An assigned Identity maintains coherent reusable operating resources precisely enough for AI reuse.

Apply the [Global Communication Rules](../../rules/global-communication-rules.md) and the [Global Writing Rules](../../rules/global-writing-rules.md).
System Rules take priority over this Skill.

## 2. NEW JOB and intake

1. Resolve the Identity during Initialization.
2. Resolve the currently authorized Responsibility and Scope from System Context.
3. Resolve record Target Locations through Identity Context and current System Rules.

Use this start order:

1. Check the latest Tab of the 03 Job Records file for an active Job.
2. Read the inbox under the [inbox](../inbox/SKILL.md) Skill.
3. Review Future Topics in Identity Context.
4. Establish the Scope.

Before interpreting a candidate's substantive Scope, read:

- Relevant Identity Context.
- Relevant scoped Knowledge Bases.
- Work Requests.
- The candidate's authoritative Closed Minutes.

## 3. Checkpoint and dependencies

1. Locate the preceding Job of the same Identity through the Jobs Chapter of the 01 Index.
2. Consult its last processed request or source checkpoint.
3. Compare identifiers only within the same sequence.
4. Preserve valid pending or excluded work.
5. Verify each dependency against Completion Notices, Requirements and sources.
6. Classify each dependency as Completed, Pending or Unverified.
7. Present unmet or unverified dependencies before Scope selection.
8. The user may authorize earlier progress within actual technical and authority limits.
9. Preserve each dependency's true state.

## 4. Scope selection

When a Task starts, the user selects the Workflow. You may propose one from the Plugin Skills and the Knowledge Bases.
If none fits, work normally under this Lifecycle.

1. A Job may consolidate several eligible Work Requests from different Identities.
2. A Job may contain several Deliverables.
3. Reconcile dependencies, overlap, supersession and conflict.
4. Each Scope keeps its originating Closed Minutes, source material and dependencies.
5. Each Deliverable keeps its originating Identity, Work Request and source references.
6. Present eligible Scope and useful combinations for the user's selection.
7. Obtain explicit confirmation of the selected Job Scope.

## 5. Future Execution work

1. Retain every valid Work Request that a confirmed Job does not wholly incorporate.
2. Keep it in the Future Topics Chapter of Identity Context.
3. Each entry has its Ref and From values, an Agent-authored Description, exact sources and relevant prerequisites.
4. Derive the Description from the request and its Minutes without duplicating the Minutes.
5. Remove unincorporated work only through explicit user direction.

## 6. Scope confirmation and Job Record

Scope confirmation permits these actions without another approval:

- Record establishment.
- Applicable Context maintenance.
- Experience search.
- Proposal preparation.

1. Confirm each Deliverable's storage place, such as Google Drive, GitHub or GitLab.
   Take it from the Final Minutes. When no place is recorded, ask the user.
2. Establish the Working Document as a new Tab in the 03 Job Records file.
   Use the [Job Records template](../../templates/job-records.md).
   Name the Tab with the tab name pattern in the Google System Rules.
3. Verify the new Tab and its Formatting under the [workflow-qa](../workflow-qa/SKILL.md) Formatting checkpoints.
4. Remove only incorporated portions from Future Topics. Retain partial and unselected remainders.
5. Save and verify the Scope confirmation.
6. Search Experiences once under the [knowledge-base](../knowledge-base/SKILL.md) Skill.

A Job may use a fresh Conversation Context. Identity Context remains durable.

## 7. Execution Plan

Prepare one comprehensive Execution Plan for the entire Job:

1. Read current target resources.
2. Analyze every included Scope and its dependencies.
3. Prepare the complete Plan.
4. Save and verify the Plan.
5. Present the saved Plan for approval.

For each confirmed Scope, the Plan identifies:

- Affected files or resources.
- Planned impacts and their reasons.
- Expected Deliverables and Outcomes.
- Each Deliverable's storage place.
- Dependencies.
- Sub-agent assignments and number.
- Model choice.
- PROFIT + A definitions under the [profit-a](../profit-a/SKILL.md) Skill.
- QA criteria.
- Completion conditions.

Include ordered execution steps for the entire Job.
The Execution List identifies target files, documents and folders.
It does not prescribe the Child's Chapters, Sections, content plan or Deliverable structure.
A structure expressly prescribed in authoritative Minutes remains binding.

## 8. PROCEED EXECUTION

1. PROCEED EXECUTION approves the complete current saved Plan once for the entire Job.
2. Save and verify the approval.
3. Ordinary refinements may remain within approved requirements.
4. A material Scope change requires a new Scope decision.
5. A material change to approved implementation requires renewed Plan approval.

## 9. Execution

1. Check the approved Plan and the required current resources.
2. Perform only authorized work.
3. Preserve unrelated content, applicable Governance and Child responsibility boundaries.
4. Search Experiences during work only for genuine difficulties, corrections or relevant quality problems.
5. A missing substantive decision returns to the Meeting process.
   Suspend the affected action until authoritative Closed Minutes resolve it.
   Preserve completed in-scope work.

## 10. Parent and Sub-agents

1. Check the actual Sub-agent creation and supervision capabilities.
2. When genuine Sub-agents are available, assign each Deliverable to a distinct genuine Sub-agent.
3. Write each Sub-agent Prompt with the complete [PROFIT + A Framework](../profit-a/SKILL.md) in Strict Mode.
4. Supply complete scoped subject knowledge, instruction-bearing Closed Minutes, constraints and supporting sources.
5. The Child determines substantive revisions, wording, organization and permitted methods.
6. The Child authors the Deliverable, performs its own QA and returns the complete candidate.
7. Sub-agents do not modify the Job Record.
8. Review the entire candidate at every submission against sources, Requirements, the Global Writing Rules and artifact quality rules.
9. A FAIL requires specific feedback.
10. Allow at most five Child retries after the initial submission.
11. After five failed retries, report the unpassed outcome for the user's decision.
12. Do not assume the Child's substantive authorship.

When genuine Sub-agents are unavailable:

1. The Parent authors the Deliverable.
2. It performs a separate complete review pass.
3. It labels the work as not delegated in the Job Record.

Never represent a simulated Child as genuine delegation.
Follow model decisions from authoritative Minutes. Otherwise offer the models available in the environment for user selection.
Past choices may inform nonbinding advisory Proposals.

## 11. Acceptance and recording

1. Only a fully accepted candidate proceeds to saving, publication, Job Record entry or Completed status.
2. Temporary review copies are not accepted Deliverables.
3. Record each Deliverable as soon as it is accepted and saved.
4. Include its exact location, source and originating Identity.
5. Preserve actual changes, outcomes, Deliverable types, locations and evidence.
6. Save and verify accepted results and relevant evidence.

## 12. Completion

Complete these steps in order:

1. Perform internal QA under the [workflow-qa](../workflow-qa/SKILL.md) quality dimensions.
   Verify the saved Deliverables and their Job Record entries.
2. Verify the complete final Job Record.
3. Finalize the Job Record with the Completion Report, QA evidence and actual Job Done Time.
4. Freeze the completed Job Record as Proof of Job.
5. Add one Jobs row to the 01 Index. Verify the row.
   The From cell names the sending Meeting and its record key, linked to that record.
6. Update Identity Context.
7. Optionally maintain relevant verified Knowledge Base content within approved authority.
8. Capture Experience once for the entire Job under the [knowledge-base](../knowledge-base/SKILL.md) Skill.
9. Send relevant Completion Notices last under the [inbox](../inbox/SKILL.md) Skill.

Apply System Rules to actual persistence and indexing.
Preserve each Deliverable's own outcome and verification status across Scopes and Identities.
Self-verification does not replace an independent QA Workflow.

## 13. Completion Notice recipients

1. Send a Completion Notice to each originating Identity.
2. Determine notices through each Deliverable's original Scope and Identity.
3. Review every incorporated Work Request and its sources.
4. Notify other registered Identities whose current Responsibilities intersect the outcome.
5. Avoid unrelated or duplicate notices.

## 14. Local and remote environments

Local working is hybrid. Google Drive remains the authority.

1. Preserve authoritative Google decisions, approved Scope, the Plan, Agent boundaries and approvals.
2. Keep System Context, Identity Context, the index and the inbox in Google.
3. Follow the Local System Rules for the local folder and for when and how work returns to Google.
4. Return the Job Record to Google at Job completion, before step 5 of Section 12.
5. Store each Deliverable in its agreed place.
6. Index or announce nothing until its record is in Google and its Deliverable is in the agreed place.
7. Verify required updates before claiming completion.
8. Report unavailable access or uncompleted updates accurately. Discuss permitted setup with the user.

## 15. System resource changes

1. Perform authorized System resource updates only within an approved Job Scope.
2. Preserve each affected Scope's working state, Governance, assignments and customization.
3. Preserve active work, records and valid pending requests.
4. Verify affected resources and outcomes independently.

## 16. Stage words

NEW JOB and PROCEED EXECUTION are the user's stage words.
This Skill holds the full flow of each stage.
A stage word does not autonomously trigger work or expand authority.
