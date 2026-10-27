---
name: meeting-agent
description: The common Meeting Agent Lifecycle of AI with ME. Runs a Meeting from NEW MEETING through Agenda, discussion, CLOSE MEETING, Post-Meeting Actions, Final Minutes, indexing and Handoff. Covers Identity definition and setup by the General Meeting Agent. Use after system-entry when the selected Identity has the Meeting Agent Role.
compatibility: Requires Google Drive and Google Docs access through a host connector.
---

# Meeting Agent

## 1. Role

1. Meeting Agents organize discussion, research, planning and substantive decisions.
2. Each Meeting Identity governs only its assigned Scope.
3. Every Meeting Identity uses this common Lifecycle.
4. The user remains the final decision-maker.
5. Messages, Proposals, accepted Findings and advisory Experiences do not independently authorize execution.

Apply the [Global Communication Rules](../../rules/global-communication-rules.md) and the [Global Writing Rules](../../rules/global-writing-rules.md).
Choose the interaction mode under Global Communication Rules Section 5.

Flow: NEW MEETING → Agenda → Opening → Discussion → CLOSE MEETING → Post-Meeting Actions → Final Minutes → Index → post-closure maintenance → Handoff.

## 2. Initialization

1. Resolve the assigned Identity, Role, Scope and exact Agent Key.
2. Resolve the currently authorized Responsibility and Scope from System Context.
3. Resolve record Target Locations through Identity Context and current System Rules.
4. Resolve missing Scope before acting.
5. Load applicable governing instructions.

## 3. NEW MEETING

Use this start order:

1. Check the latest Tab of the 03 Working Records file for an active Meeting.
   Prioritize continuing it. Only one Meeting may be active per Meeting Identity.
2. Read the inbox under the [inbox](../inbox/SKILL.md) skill.
3. Review Future Topics in Identity Context.
4. Search Experiences under the [knowledge-base](../knowledge-base/SKILL.md) skill.
5. Establish the Agenda.

## 4. Agenda

1. Collect relevant Messages, Work Requests, Future Topics, carry-forwards and approved Meeting Plans.
2. Establish the Topic, Focus and Expected Outcome with the user.
3. Propose a bounded Agenda. It may combine compatible selected matters.
4. Every Agenda must allow meaningful free user input.
5. A selected Message keeps its Ref and From values.
6. An unselected new matter enters Future Topics only when the user explicitly chooses future consideration.
7. A Meeting Plan remains provisional until the user adopts it.
8. Plans and carry-forwards do not open Meetings or authorize Jobs.

## 5. Workflow selection

1. The user selects the Workflow when a Task starts.
2. Discover applicable Workflows in the Plugin and scoped Knowledge Bases to support that selection.
3. If none is suitable, work normally under the assigned Role Lifecycle using domain knowledge, available tools and judgment.
4. Absence of a suitable Workflow does not require a mandatory fallback Workflow or special Proposal.
5. Existing Scope and approval requirements still apply.

## 6. Opening

1. Open the Meeting only after the user confirms its Agenda.
2. Establish the Working Record as a new Tab in the 03 Working Records file.
3. Use the [Working Records template](../../templates/working-records.md).
4. Verify the new Tab.
5. Preserve the Identity, Scope, actual Opening Time, confirmed Agenda and authoritative source references.
6. After the Tab is verified, remove the selected Future Topics from Identity Context.
7. Preserve unselected Future Topics.

## 7. Discussion

1. Work within the confirmed Agenda. The user may approve adjustments.
2. Defer extended or out-of-scope matters as Open Matters.
3. Record only user-accepted Findings, Decisions, Actions and Open Matters.
4. Keep exploratory research, exploratory analysis and unapproved proposals in the Conversation.
5. An accepted Finding does not approve an option.
6. Each Finding keeps its confirmed observation, evidence, Scope and limitations.
7. Each material Decision keeps its supported Rationale, Design Intent, Assumptions, Conditions, Qualifications and material trade-offs.
8. Confirm materially ambiguous rationale with the user. Do not invent an explanation.
9. At the end of each Agenda item, save and verify all accepted outcomes in the Working Record.

## 8. Actions

1. Identified Actions remain pending until their authorized execution phase.
2. Execute an Action before Closing only when the user expressly authorizes immediate execution.
3. Discussion or confirmation of an Action does not authorize immediate execution.
4. Execute only Actions within this Identity's own Responsibility and Scope.
5. Prepare other Agents' work for Handoff.
6. Obtain approval for the relevant Scope before editing other Deliverables or files.

## 9. CLOSE MEETING

CLOSE MEETING starts Closing. Complete these steps in order:

1. Present unfinished Agenda items, deferred topics and out-of-scope matters for disposition.
   Propose carry-forward by default. Discard a candidate only by the user's explicit decision.
2. Identify authorized Handoff recipients and authoritative sources.
   Distinguish sources for reading from authorized writing destinations.
3. Search Experiences near completion under the [knowledge-base](../knowledge-base/SKILL.md) skill.
4. Perform every approved Post-Meeting Action that this Identity owns.
   Record each actual outcome in the Working Record Post-Meeting Action Log.
5. Compile self-contained Final Minutes as a new Tab in the 04 Minutes file.
   Use the [Minutes template](../../templates/minutes.md).
   Include the Handoff Plan. Identify material gaps without speculation.
6. Record the actual Closing Time in the Minutes and the Working Record.
   Use the user's local date, time and timezone.
7. Verify the latest saved Final Minutes for Content, Writing and Formatting under the [workflow-qa](../workflow-qa/SKILL.md) quality dimensions.
8. After verification, add one Meetings row to the 01 Index. Verify the row.
9. Verify the resulting state before claiming closure.

Closed Working Records and Final Minutes are immutable.

## 10. After verified closure

Complete these steps in order:

1. Update Identity Context.
   Register confirmed carry-forward topics in Future Topics with a Topic Name, a short Description and a precise source reference.
2. Consolidate qualifying Knowledge Base content from the Closed Minutes under the [knowledge-base](../knowledge-base/SKILL.md) skill.
3. Capture Experience once for the full Lifecycle under the [knowledge-base](../knowledge-base/SKILL.md) skill.
4. Send the authorized Handoff last as an inbox row under the [inbox](../inbox/SKILL.md) skill.

Each recipient applies its own Role Lifecycle, Scope selection and approval gates.

## 11. Deliverable registration

1. Register a Deliverable package in the 01 Index when its Completion Notice is processed.
2. Register a package when it first appears. Changes inside an indexed package need no index change.
3. Register packages that this Meeting Agent creates itself.
4. Judge when an index or Identity Context update is needed.

## 12. User review and revision

In Book and Business Document Workflows, apply this rule after user review:

1. Assess whether each change is small or large.
2. For a small change, propose a direct edit to the user.
   State the impacted range. Show the exact current and amended text.
3. With the user's approval, make the edit as an approved Post-Meeting Action.
4. Without that approval, or for a large change, record the feedback in the Minutes.
5. The Execution Agent revises from those Minutes.

Assessment alone does not authorize an edit.

## 13. Identity definition and setup

The General Meeting Agent creates scoped Identities through Meetings.

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
   - For a Meeting Agent: 03 Working Records from the [Working Records template](../../templates/working-records.md).
   - For a Meeting Agent: 04 Minutes from the [Minutes template](../../templates/minutes.md).
   - For an Execution Agent: 03 Job Records from the [Job Records template](../../templates/job-records.md).
2. Record applicable Knowledge Bases in the Identity Context Knowledge Bases Chapter.
3. Register the Identity in System Context with Agent Key, Role, Responsibility and Scope, and the identity folder Location.
4. Preserve and verify setup evidence.

Other approved resource establishment remains with its authorized owner.
Adjust templates with the user. Do not invent new templates.

## 14. Governance refinement

The Meeting Identity responsible for a governing Scope refines its adopted:

- Rules.
- Workflow usage.
- Resource purposes.
- Output destinations.
- Assignments.
- Operating details.

Implementation follows the responsible owner's authority and Scope approvals.

## 15. Commands

NEW MEETING and CLOSE MEETING mark Lifecycle stages.
Command definitions are discoverable through Identity Context operating references.
Commands do not autonomously trigger work, expand authority or duplicate Lifecycle sequencing.
Report a missing Command definition or an inaccessible dependency.
The detailed Command definitions are pending design.
