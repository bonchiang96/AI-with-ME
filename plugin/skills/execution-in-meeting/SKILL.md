---
name: execution-in-meeting
description: The AI with ME Execution in Meeting guideline. Suggests how a Meeting Agent makes a Deliverable with its own Sub-agents inside a Meeting. Covers the suggested Agenda, the Plan, how Sub-agents divide the work, AI review and human review. Use in a Meeting Job when the Deliverable Guideline sets no way of working.
compatibility: Requires the Google Drive and Google Docs connectors through the host. The Plugin does not ship the connectors.
---

# Execution in Meeting guideline

## 1. Nature of this guideline

1. This Skill is a guideline. It tells you what you can do. Adapt it to the situation.
2. Rules stay fixed. Apply the [global-writing-rules](../global-writing-rules/SKILL.md) and [global-communication-rules](../global-communication-rules/SKILL.md) Skills unchanged.
3. The Meeting runs the Meeting flow of the [meeting-agent](../meeting-agent/SKILL.md) Skill. This guideline works inside that flow.
4. When the Deliverable Guideline sets the way of working, follow its way.
   It sets arrangements such as the Agenda items, the number of workers and the number of reviewers.
5. When the Deliverable Guideline sets no way of working, follow this guideline.
   Rationale: every Deliverable has a different way of working. This default guides Deliverable work whose Guideline sets no way of working.

## 2. Suggested Agenda

Suggest these Agenda items for a Meeting that makes a Deliverable:

1. **Plan.** Study the Deliverable Guideline and present a Plan under Section 3.
2. **Making.** Sub-agents make the Deliverable under Section 4.
3. **AI review.** A reviewer Sub-agent reviews the saved Deliverable under Section 5.1.
4. **Human review.** The user reviews the Deliverable under Section 5.2.

AI review and human review may be two Agenda items or one.
The user may set the later Agenda items before the Meeting starts.
The Agenda may change during the Meeting. An example is a return to the Deliverable for revision after a review.

## 3. Plan

1. Study the Job Scope sources in Authoritative Sources of the Meeting Record.
   They are the Deliverable Guideline, the Closed Minutes and the relevant Knowledge Bases.
   Also study the current target resources.
2. Prepare the Plan yourself, or assign a planner Sub-agent to prepare it.
3. The Plan lists each Deliverable item with its Sub-agents, its review and its pause points.
   A pause point is a place where Sub-agents stop for the user.
4. Present the Plan item by item. Discuss each adjustment with the user.
5. Record the agreed Plan as a Decision in the Meeting Record.

## 4. Making the Deliverable

1. Assign worker Sub-agents under the Plan.
   Use the Sub-agent mechanisms of the [execution-agent](../execution-agent/SKILL.md) Skill Section 10 items 1 to 6.
2. Each worker's Feed holds the Deliverable Guideline, the Closed Minutes, the Knowledge Base content and the current target resources.
3. A reviewer Sub-agent should review each candidate.
   You should accept each candidate on the reviewer's last report, without your own review.
   Rationale: your context holds the whole Meeting. A reviewer Sub-agent has a clean context.
4. Send the reviewer's findings to the worker. The reviewer then checks again.
5. At each pause point, show the worker's work to the user before any acceptance review.
   Pass the user's input to the same worker. The worker continues.

## 5. Review

### 5.1 AI review

1. Assign a reviewer Sub-agent to review the saved Deliverable.
   It covers fidelity, the Global Writing Rules and presentation style.
2. Its Feed holds the Deliverable, the Deliverable Guideline, the Closed Minutes and the review Decisions of this Meeting.
3. Rationale: your context holds the whole Meeting. A reviewer Sub-agent has a clean context.

### 5.2 Human review

1. Present the saved Deliverable and the reviewer's report to the user.
2. Give the user Agenda space for the user's own review.
3. Consolidate the reviewer's report and the user's review.

### 5.3 Revision

1. Turn each review Decision that changes the Deliverable into an edit instruction.
2. Send the instruction to the original worker to continue, or to a new worker.
3. The Prompt carries the Deliverable Guideline, the current Deliverable and the review Decisions of this Meeting.
4. A reviewer Sub-agent checks the edited candidate. It checks again after its findings are applied.
5. Continue with AI review and human review of the edited Deliverable.
