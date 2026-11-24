# Execution in Meeting guideline

Return to the [Requirements Overview](../README.md).

## 1. Nature and use

1. **Guideline.** This file is a guideline under [Requirements Overview Section 1.6](../README.md#1-framework-definition).
   It tells the Meeting Agent what it can do in a Meeting Job. The Meeting Agent may adapt it to the situation.
   The Global Writing Rules and the Global Communication Rules stay fixed.

2. **Place in the Meeting flow.** The Meeting Job runs the Meeting flow under [Meeting Lifecycle Section 6](../03-meeting-lifecycle.md#6-meeting-job).
   This guideline works inside that flow.

3. **Priority.** When the Deliverable Guideline sets the way of working, the Meeting Job follows its way.
   The Deliverable Guideline sets arrangements such as the Agenda items, the number of workers and the number of reviewers.
   When no Deliverable Guideline sets the way of working, the Meeting Job follows this guideline.
   Rationale: every Deliverable has a different way of working. This default guides a Meeting Job whose Deliverable Guideline sets no way of working.

4. **Packaging.** The Plugin packages this guideline as the execution-in-meeting Skill.

## 2. Suggested Agenda

1. **Agenda items.** For a Meeting that makes a Deliverable, the Meeting Agent should suggest these Agenda items:

   1. Plan: study the Deliverable Guideline and present a Plan under [Section 3](#3-plan).
   2. Making: Sub-agents make the Deliverable under [Section 4](#4-making-the-deliverable).
   3. AI review: a reviewer Sub-agent reviews the saved Deliverable under [Section 5.1](#5-review).
   4. Human review: the user reviews the Deliverable under [Section 5.2](#5-review).

   AI review and human review may be two Agenda items or one.

2. **Agenda changes.** The user may set the later Agenda items before the Meeting starts.
   The Agenda may change during the Meeting. An example is a return to the Deliverable for revision after a review.

## 3. Plan

1. **Sources.** Study the Job Scope sources in Authoritative Sources of the Meeting Record.
   They are the Deliverable Guideline, the Closed Minutes and the relevant Knowledge Bases.
   Also study the current target resources.

2. **Preparation.** The Meeting Agent prepares the Plan itself or assigns a planner Sub-agent.
   The Plan lists each Deliverable item with its Sub-agents, its review and its pause points.
   A pause point is a place where Sub-agents stop for the user.

3. **Agreement.** Present the Plan item by item. Discuss each adjustment with the user.
   Record the agreed Plan as a Decision in the Meeting Record.

## 4. Making the Deliverable

1. **Workers.** Assign worker Sub-agents under the Plan.
   Use the Sub-agent mechanisms under [Execution Lifecycle Section 4](../04-execution-lifecycle.md#4-execution-parent-and-sub-agents).
   Each worker's Feed holds the Deliverable Guideline, the Closed Minutes, the Knowledge Base content and the current target resources.

2. **Reviewer.** A reviewer Sub-agent should review each candidate.
   The Parent should accept each candidate on the reviewer's last report, without its own review.
   Rationale: the Parent's context holds the whole Meeting. A reviewer Sub-agent has a clean context.

3. **Findings.** The worker acts on the reviewer's findings. The reviewer then checks again.

4. **Pause points.** At each pause point, show the worker's work to the user before any acceptance review.
   Pass the user's input to the same worker. The worker continues.

## 5. Review

1. **AI review.** A reviewer Sub-agent reviews the saved Deliverable for fidelity, the Global Writing Rules and presentation style.
   Its Feed holds the Deliverable, the Deliverable Guideline, the Closed Minutes and the review Decisions of the Meeting.
   Rationale: the Parent's context holds the whole Meeting. A reviewer Sub-agent has a clean context.

2. **Human review.** Present the saved Deliverable and the reviewer's report to the user.
   Give the user Agenda space for the user's own review. Consolidate both reviews.

3. **Revision.** Each review Decision that changes the Deliverable becomes an edit instruction.
   Send it to the original worker or to a new worker.
   The Prompt carries the Deliverable Guideline, the current Deliverable and the review Decisions of the Meeting.
   A reviewer Sub-agent checks the edited candidate. It checks again after its findings are applied.
   Continue with AI review and human review of the edited Deliverable.
