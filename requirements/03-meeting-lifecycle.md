# Meeting Lifecycle

Return to the [Requirements Overview](README.md).

## 1. Initialization and preparation

1. **Initialization.** Resolve the assigned:

   - Identity.
   - Role.
   - Scope.
   - Exact Agent Key.

   Load applicable governing instructions.
   At NEW MEETING, use this start order:

   1. Check for an active Meeting under [Section 1.2](#1-initialization-and-preparation).
   2. Read the inbox under [Records, Messaging and Experiences Section 2.6](05-records-messaging-and-experiences.md#2-messaging).
   3. Review Future Topics. A Future Topic named "Meeting Job: <Deliverable>" hands Deliverable work to this Meeting under [Section 6](#6-meeting-job).
   4. Search Experiences under [Records, Messaging and Experiences Section 3.3](05-records-messaging-and-experiences.md#3-experience-learning).
   5. Establish the Agenda under [Section 1.3](#1-initialization-and-preparation).

   Guidance: with an empty Identity Context and no Knowledge Base, the Meeting Agent starts with information gathering about the Scope.
   At NEW MEETING, it may propose to collect information about the Scope with the user.

2. **Active Meeting continuity.** An active Meeting is a Meeting without Final Minutes. A Meeting with Final Minutes is closed.
   At NEW MEETING, first check the latest Tab of the Meeting Records file for an active Meeting. Prioritize continuing it.
   Each Meeting Identity may have only one active Meeting at a time.

3. **Agenda sources.** After reading the inbox, collect relevant:

   - Messages.
   - Work Requests.
   - Future Topics.
   - Carry-forwards.
   - Approved Meeting Plans.

   Establish the following with the user:

   - Topic.
   - Focus.
   - Expected Outcome.

   Propose a bounded Agenda that may combine compatible selected matters.
   Every Meeting Agenda must allow meaningful free user input.

   Making a Deliverable is one Agenda item. A review Agenda item may follow it.
   The Agenda items follow the way of working under [Section 6.1](#6-meeting-job). A Meeting may make several Deliverables.

   The proposed Agenda shows each Job Scope.
   A Job Scope holds the Deliverable, its storage place, the Guideline link, the latest Closed Minutes and the relevant Knowledge Bases.
   The Job Scope comes from the Deliverable Guideline and the place where it is stored.
   The user's Agenda confirmation confirms each Job Scope. It starts the Deliverable work.

4. **Message selection.** A Message selected for the current Agenda must retain its Ref and From values.
   Unselected new matters enter Future Topics only when the user explicitly chooses future consideration.

   Each inbox row's matter gets one place: the Agenda, Future Topics, or no place.
   No place applies when the user says the matter is not needed.
   Every inbox Type follows this rule. The row stays in the inbox until its matter has its place.

   Apply the user-supplied Context rule in [Foundation Section 3.5](01-foundation.md#3-identity-context).

5. **Opening.** Open the Meeting only after the user confirms its Agenda. Establish its Meeting Record as a new Tab in the Meeting Records file.
   Every Meeting uses the next M key, including a Meeting that makes a Deliverable.
   The next key comes from the Meetings Chapter of the index.

   With an Agent workspace, the Tab is the entry record. The Meeting Record continues in the workspace under [Environments and Acceptance Section 2.9](07-environments-and-acceptance.md#2-hybrid-local-working-and-deliverable-storage).
   The Final Minutes are drafted there and sync to Google at Meeting close.
   Name the Tab under the tab name pattern in [Foundation Section 2.4](01-foundation.md#2-governance-resources-and-dependencies). Verify that resource.

   Preserve:

   - Assigned Identity and Scope.
   - Actual Opening Time.
   - The confirmed Agenda.
   - Authoritative source references.

   For each Deliverable on the Agenda, copy its Job Scope sources into Authoritative Sources.
   They are the latest Closed Minutes link, the Guideline link and the storage place.

6. **Future Topic transfer.** Remove selected existing Future Topics only after their new Meeting Record is successfully established. Preserve unselected entries.
   After the Meeting Record is established, complete these steps:

   1. Record each matter chosen for Future Topics in Confirmed Agenda, with its Ref and From values.
   2. Delete each inbox row whose matter is in the Agenda.
   3. Delete each inbox row whose matter the user said is not needed.

   A row whose matter goes to Future Topics is deleted after the Future Topics are saved under [Section 3.5](#3-closing-and-handoff).

## 2. Discussion and outcomes

1. **Agenda boundaries.** Work within the confirmed Agenda. The user may approve adjustments. Defer extended or out-of-scope matters as Open Matters rather than independently expanding the discussion.

2. **Accepted outcomes.** Meeting records must distinguish these user-accepted outcomes:

   - Findings.
   - Decisions.
   - Actions.
   - Open Matters.

   The following remain in Conversation:

   - Exploratory research.
   - Exploratory analysis.
   - Unapproved proposals.

   Record in two steps. First record the user's answer to each question the Agent asked.
   Then judge whether other content is worth recording within the Topic and Scope.
   Record it as a Finding, a Decision or a Rationale only when it is. Leave out the rest.

   A user's example, imagined situation or thinking aloud is not a Decision.
   When the Agent cannot tell whether a statement is a Decision, ask the user.
   This rule covers the user's own Findings and Decisions. Sub-agent reports follow [Section 6.2](#6-meeting-job).

   An accepted Finding does not automatically approve an option.

3. **Preserved meaning.** Accepted Findings must retain relevant:

   - Confirmed observation.
   - Evidence.
   - Scope.
   - Limitations.

   Findings do not require mandatory Rationale or Design Intent.
   Material Decisions keep their User's words by the source of the Decision under [Global Communication Rules Section 2.8](global-communication-rules.md#2-language).
   Material Decisions must also preserve supported:

   - Rationale.
   - Design Intent.
   - Assumptions.
   - Conditions.
   - Qualifications.
   - Material trade-offs.

   A Rationale may hold the Agent's own reasoning.
   When the Agent is unsure whether a Rationale or a point matches the user's meaning, ask the user.

4. **Persistence checkpoints.** At the end of each Agenda item, save and verify all accepted outcomes in the Meeting Record.
   Intermediate saving within an Agenda item is discretionary.
   The Meeting Record's persistence and QA boundary follows [Quality Section 1.1](06-quality.md#1-deliverable-quality-and-independent-qa).

5. **Learning Candidates.** Record each user correction or stated success as a Learning Candidate in the Meeting Record when it happens.
   Learning Candidates follow [Records, Messaging and Experiences Section 3.6](05-records-messaging-and-experiences.md#3-experience-learning).

6. **Deliverable arrangement.** For each Deliverable, agree its storage place with the user and ask for the path or location.
   When the Meeting decides a Deliverable, it discusses the Deliverable Guideline content. The Meeting Record then holds everything the Guideline needs.
   Propose the Deliverable Guideline arrangement under [Foundation Section 4.12](01-foundation.md#4-scoped-knowledge-base).
   The user confirms it.

   Agree with the user who executes each Deliverable: an Execution Identity or this Meeting Agent.

   When this Meeting Agent executes, the Guideline content may set the Execution arrangement:

   - The Agenda items that make the Deliverable.
   - The Sub-agent roles and their number, such as worker and reviewer.
   - When a reviewer steps in, and who acts on its findings.
   - Whether the Parent reviews.
   - Where Sub-agents continue and where they stop for the user. Each stop is a pause point.

   The Meeting Agent may adapt the Execution arrangement to the situation under [Requirements Overview Section 1.6](README.md#1-framework-definition).

   A Meeting can make or change a Deliverable when its Deliverable Guideline exists.
   The Guideline holds the concept of the Deliverable.

   - When the Guideline exists, the Meeting makes or changes the Deliverable.
     Each change that affects the Guideline is recorded as a Decision of the Meeting.
     The Deliverable follows the latest Decisions.
     After close, these Decisions are edited into the Guideline or a Knowledge Base under [Section 3.7](#3-closing-and-handoff).
   - When no Guideline exists, the Meeting discusses the Guideline content.
     The Guideline is created after close. A later Meeting makes the Deliverable.

7. **Actions.** Identified Actions remain pending until their authorized execution phase unless the user explicitly authorizes earlier execution. Execute only actions within the Meeting Identity's own Responsibility and Scope. Prepare other Agents' work for handoff.
   Making a Deliverable in a Meeting is not an Action. It happens in Agenda items under [Section 6](#6-meeting-job).

## 3. Closing and handoff

1. **Closing dispositions.** At CLOSE MEETING, present the following for disposition:

   - Unfinished Agenda items.
   - Deferred topics.
   - Out-of-scope matters.

   Carry-forward is the default proposal. Discard a candidate only through the user's explicit decision.

2. **Final Minutes.** Compile self-contained Final Minutes under [Section 5](#5-meeting-artifacts) after completing the approved actions in [Section 4](#4-post-meeting-actions).
   Preserve essential constraints and supported outcomes.
   Include the intended Handoff Plan.

   Include the full Guideline content for each Deliverable the Meeting decided.
   For each Deliverable the Meeting decided, include the executor and any Execution arrangement.
   When a later Meeting makes it, the Handoff Plan names its Future Topic as the Handoff.
   For Deliverable work in the Meeting, include the agreed Plan, the accepted Deliverables, the review Decisions and the Stable Decision.

   Record each Deliverable's storage place under [Environments and Acceptance Section 2.6](07-environments-and-acceptance.md#2-hybrid-local-working-and-deliverable-storage).
   Identify material gaps without speculation.
   Later Execution reads Final Minutes for applicable instructions without requiring access to the internal live Meeting Record.

3. **Closing order.** At CLOSE MEETING, complete these steps in order:

   1. Present matters for disposition under [Section 3.1](#3-closing-and-handoff).
   2. Identify authorized recipients and authoritative sources under [Section 3.7](#3-closing-and-handoff).
   3. Search Experiences under [Records, Messaging and Experiences Section 3.3](05-records-messaging-and-experiences.md#3-experience-learning).
   4. Complete approved Post-Meeting Actions under [Section 4.3](#4-post-meeting-actions).
   5. Compile the Final Minutes under [Section 3.2](#3-closing-and-handoff).
   6. Record the actual Closing Time consistently in Minutes and the Meeting Record.
   7. Run writing checking on the Final Minutes in their final version under [Quality Section 1.3](06-quality.md#1-deliverable-quality-and-independent-qa).
   8. Save the Meeting Record and Final Minutes to Google. With an Agent workspace, run the completion sync.
   9. Run the save checks on the saved Final Minutes under [Quality Section 1.3](06-quality.md#1-deliverable-quality-and-independent-qa).
   10. Add the index row under [Section 3.4](#3-closing-and-handoff).
   11. Clean the Meeting's workspace folder under [Environments and Acceptance Section 2.16](07-environments-and-acceptance.md#2-hybrid-local-working-and-deliverable-storage).

   Complete substantive closing work and required artifact checks before finalizing closure.

   Use the user's applicable local:

   - Date.
   - Time.
   - Time-zone abbreviation.

   Preserve closed Meeting records and Minutes as immutable records.

4. **Indexed closure.** After the Final Minutes are verified, add one Meetings row to the index under [Foundation Section 5.3](01-foundation.md#5-identity-folder-index-and-inbox).
   The row uses the M key.

   For each Deliverable made in the Meeting, then register or update its package.
   Verify each row.
   The package's Condition is Stable when the user decided Stable in the Meeting. Otherwise it is Draft.
   Rationale: the Meeting Record and the Final Minutes reach Google at Meeting close.

   Indexing follows [Environments and Acceptance Section 2.8](07-environments-and-acceptance.md#2-hybrid-local-working-and-deliverable-storage).
   Verify the resulting state before claiming closure.

5. **Future Topics.** After verified closure, register confirmed carry-forward topics in the owning Identity Context Future Topics Chapter.

   Each entry needs:

   - A Topic Name.
   - A short Description.
   - A precise source reference.

   Include each matter recorded for Future Topics at Opening.
   When a later Meeting makes a Deliverable decided in the Meeting, its Future Topic is named "Meeting Job: <Deliverable>".
   Its source references are the Closed Minutes, the Deliverable Guideline link and the storage place.
   This Future Topic hands the Deliverable work to a later Meeting.
   After the Future Topics are saved, delete each inbox row whose matter they now hold.

   Keep one readable list. Exclude:

   - Independent topic statuses.
   - Counters.
   - Removal history.

6. **Meeting Plans.** A Meeting Plan remains provisional future work until the user adopts it. Plans and carry-forwards do not automatically open Meetings or authorize Jobs.

7. **Final Handoff.** Identify authorized recipients and authoritative sources before closure.
   Distinguish sources for reading from authorized writing destinations.

   Complete the following in order after verified Meeting closure:

   1. Consolidate qualifying scoped Knowledge Base content under [Foundation Section 4](01-foundation.md#4-scoped-knowledge-base).
      In the same step, create the Deliverable Guideline for each Deliverable the Meeting decided.
      Write it from the Closed Minutes in its agreed place.
      Consolidate each other affected Deliverable Guideline in the same step under [Foundation Section 4.12](01-foundation.md#4-scoped-knowledge-base).
      Each Decision of the Meeting that affects a Guideline reaches it in this step.
   2. Perform full-lifecycle Experience Capture under [Records, Messaging and Experiences Section 3](05-records-messaging-and-experiences.md#3-experience-learning).
   3. Update Identity Context in one step under [Foundation Section 3.14](01-foundation.md#3-identity-context).
      Include Future Topics, Working Group, Important Learning and Important Things or High-Priority Items.
   4. Send the authorized Handoff last as an inbox row under [Records, Messaging and Experiences Section 2](05-records-messaging-and-experiences.md#2-messaging).
      A Handoff for Deliverable work names the Deliverable Guideline link and the latest Closed Minutes.
      Deliverable work handed to a later Meeting has its Handoff in a Future Topic under [Section 3.5](#3-closing-and-handoff).
      It needs no inbox row.
      This work sends no Completion Notice.

   Each recipient applies its own Role Lifecycle, Scope selection and approval gates.

## 4. Post-Meeting Actions

1. **Own operating resources.** Meeting Identities maintain their own Context and current Meeting Records within governing rules.
   They may maintain applicable shared Knowledge Bases within their Responsibility and Scope.
   Identity Context maintenance follows [Foundation Section 3](01-foundation.md#3-identity-context).
   Knowledge Base maintenance follows [Foundation Section 4](01-foundation.md#4-scoped-knowledge-base).

2. **Other Deliverables.** Before editing other Deliverables or files, the Meeting Identity must obtain approval for the relevant Scope.
   Authority depends on Responsibility and approval, regardless of amendment size or file type.
   Ownership follows [System, Identity and Entry Section 2.10](02-system-identity-and-entry.md#2-agent-responsibilities-stage-words-and-workflows).

3. **Closing transition.** CLOSE MEETING initiates Closing and normal approved Post-Meeting Action execution.
   Finish every approved, Meeting-Agent-owned Post-Meeting Action before compiling Final Minutes.
   Preserve each action's actual outcome in the Meeting Record.
   Other Identities' work remains a separate authorized Handoff.
   Post-closure Knowledge Base consolidation follows [Foundation Section 4.8](01-foundation.md#4-scoped-knowledge-base).
   Apply the finalized record requirements in [Section 3.3](#3-closing-and-handoff).

4. **Immediate execution.** Before Closing, execute an identified action only when the user expressly authorizes immediate execution.

   Discussion or confirmation of a required action alone does not authorize immediate execution.

## 5. Meeting artifacts

1. **Separate purposes.** Every Meeting must have an internal Meeting Record and separate user-facing Final Minutes.
   The Meeting Record supports durable Agent continuity.
   Final Minutes provide a consolidated, independently readable account.

2. **Shared metadata.** Both artifacts must identify:

   - Meeting ID, an M key.
   - Identity.
   - Role.
   - Topic.
   - Focus.
   - Expected Outcome.
   - Status, Active or Closed under [Section 1.2](#1-initialization-and-preparation).
   - Opening Time.
   - Closing Time.

3. **Meeting Record.** The append-oriented Meeting Record must primarily follow the confirmed Agenda.
   It must have five functional Chapters:

   1. Meeting Information.
   2. Confirmed Agenda.
   3. Agenda Outcomes.
   4. Post-Meeting Action Log.
   5. Authoritative Sources.

   Preserve accepted outcomes under [Section 2](#2-discussion-and-outcomes) rather than a conversation transcript.
   Persistence follows [Section 2.4](#2-discussion-and-outcomes).
   For Deliverable work, the Meeting Record also holds its content under [Section 6.2](#6-meeting-job).

4. **Final Minutes.** Final Minutes must have five Chapters:

   1. Meeting Information & Agenda.
   2. Confirmed Findings & Decisions.
   3. Actions & Outcomes.
   4. Open Matters & Dispositions.
   5. Sources & Quality Verification.

   Findings and Decisions share one substantive Chapter.
   Preserve their respective meaning under [Section 2.3](#2-discussion-and-outcomes).
   Final Minutes record their Meeting Record Locator.
   Final Minutes use Strict Mode under [Global Writing Rules](global-writing-rules.md).
   They must pass full Content, Writing and Formatting verification under [Quality Section 1](06-quality.md#1-deliverable-quality-and-independent-qa).

5. **Minutes organization.** The Meeting Agent determines the internal subject grouping, heading hierarchy, order and presentation.
   Organize Final Minutes by related subject matter without requiring Agenda chronology.
   Related outcomes from different Agenda items may be consolidated.
   Preserve the full adopted substance.

## 6. Meeting Job

1. **Purpose.** Meeting Job is a concept. It names a Meeting doing Deliverable work with the Meeting Agent's own Sub-agents.
   Every Meeting follows the same Meeting flow. Making the Deliverable is one Agenda item. A review Agenda item may follow it.
   [Section 2.6](#2-discussion-and-outcomes) sets when a Meeting can make a Deliverable.

   The Parent is the Meeting Agent. The Parent assigns Sub-agents inside the Agenda item.
   The Sub-agents share the Identity's Identity Context.

   When the Deliverable Guideline sets the way of working, the Meeting Agent follows its way.
   When the Deliverable Guideline sets no way of working, the Meeting Agent follows the [Execution in Meeting guideline](guidelines/execution-in-meeting.md).
   The Meeting Agent uses [Execution Lifecycle Section 4](04-execution-lifecycle.md#4-execution-parent-and-sub-agents) only for its Sub-agent mechanisms.

2. **Record.** Deliverable work in a Meeting has no Job Record. The Meeting Record of the Meeting is its record.
   The Parent records every Sub-agent report and result in the Meeting Record as a Finding, a Decision or an Action.
   These records need no user acceptance.
   Rationale: every action and edit of a Sub-agent must have a record.

   The record holds the report content itself. A local path or a short summary alone does not preserve it.
   The agreed Plan and the user's input at each pause point are recorded as Decisions.
   Sub-agents do not modify the Meeting Record.
   With an Agent workspace, the Sub-agents' working files stay in the Meeting's workspace folder.

3. **Making the Deliverable.** The user's Agenda confirmation has confirmed the Job Scope.
   The Experience search at NEW MEETING serves this work. Complete these steps in order:

   1. Read the Job Scope from Authoritative Sources in the Meeting Record.
   2. Work through the Agenda items in the way of working under [Section 6.1](#6-meeting-job).
   3. A missing substantive decision is discussed in the Meeting and recorded as a Decision.
   4. Save each accepted Deliverable in its agreed place.
      Run the save checks under [Quality Section 1.3](06-quality.md#1-deliverable-quality-and-independent-qa).
   5. Record each accepted Deliverable as an Action with its exact location and outcome.

   The user reviews the Deliverable at pause points and in review Agenda items.

4. **Review.** A review Agenda item judges the Deliverable as a Meeting Agent.
   AI review and human review may be separate Agenda items.

   1. A review may make new Decisions. A new Decision may change an earlier Decision.
   2. A Decision that a review makes is decision making inside the Meeting.
      It is recorded with each Finding under [Section 2](#2-discussion-and-outcomes).
   3. A review Decision authorizes its edit.
   4. Until the Meeting closes, the review Decisions stand in for the consolidated Guideline.
   5. In a Workflow with numbered drafts, each edit round produces the next numbered draft.
   6. Each accepted edited Deliverable is saved and passes the save checks.
   7. Each edit round is recorded with its time, Decision reference, instruction and Sub-agent report content.
   8. The review ends when the user says the Deliverable is OK.
      Ask whether this version is the Stable version. Record the answer as a Decision.
   9. After the user's OK, no further writing checking runs unless the user asks.

   Review Decisions reach the Guideline through the Closed Minutes at post-closure consolidation under [Section 3.7](#3-closing-and-handoff).

5. **Number of Deliverables.** A Meeting may make any number of Deliverables.
   The Identity may also hand the work to an Execution Identity.
