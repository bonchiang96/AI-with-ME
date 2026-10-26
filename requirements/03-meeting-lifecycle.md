# Meeting Lifecycle

Return to the [Requirements Overview](README.md).

## 1. Initialization and preparation

1. **Initialization.** Resolve the assigned:

   - Identity.
   - Role.
   - Scope.
   - Exact Agent Key.

   Load applicable governing instructions. When Messaging is enabled, preserve Initialization RECEIVE AGENT MESSAGES and NEW MEETING READ MESSAGES as distinct checkpoints.

2. **Active Meeting continuity.** At NEW MEETING, first search for an existing active Meeting and prioritize continuing it. Each Meeting Identity may have only one active Meeting at a time.

3. **Agenda sources.** Collect relevant:

   - Messages.
   - Work Requests.
   - Future Meeting Topics.
   - Carry-forwards.
   - Approved Meeting Plans.

   Establish the following with the user:

   - Topic.
   - Focus.
   - Expected Outcome.

   Propose a bounded Agenda that may combine compatible selected matters.
   Every Meeting Agenda must allow meaningful free user input.

4. **Message selection.** A Message selected for the current Agenda must retain its identifier and source.
   Unselected new matters enter Future Topics only when the user explicitly chooses future consideration.
   Apply the user-supplied Context rule in [Foundation Section 3.5](01-foundation.md#3-identity-context).

5. **Opening.** Open the Meeting only after the user confirms its Agenda. Establish its Working Record and optional index. Verify those resources.

   Preserve:

   - Assigned Identity and Scope.
   - Actual Opening Time.
   - The confirmed Agenda.
   - Authoritative source references.

6. **Future Topic transfer.** Remove selected existing Future Topics only after their new Meeting Record is successfully established. Preserve unselected entries.

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

   An accepted Finding does not automatically approve an option.

3. **Preserved meaning.** Accepted Findings must retain relevant:

   - Confirmed observation.
   - Evidence.
   - Scope.
   - Limitations.

   Findings do not require mandatory Rationale or Design Intent.
   Material Decisions must preserve supported:

   - Rationale.
   - Design Intent.
   - Assumptions.
   - Conditions.
   - Qualifications.
   - Material trade-offs.

   Confirm materially ambiguous rationale rather than inventing an explanation.

4. **Persistence checkpoints.** At the end of each Agenda item, save and verify all accepted outcomes in the Working Record.
   Intermediate saving within an Agenda item is discretionary.
   Ordinary content changes do not require Database index updates.
   The Working Record's persistence and QA boundary follows [Quality Section 1.1](06-quality.md#1-deliverable-quality-and-independent-qa).

5. **Actions.** Identified Actions remain pending until their authorized execution phase unless the user explicitly authorizes earlier execution. Execute only actions within the Meeting Identity's own Responsibility and Scope. Prepare other Agents' work for handoff.

## 3. Closing and handoff

1. **Closing dispositions.** At CLOSE MEETING, present the following for disposition:

   - Unfinished Agenda items.
   - Deferred topics.
   - Out-of-scope matters.

   Carry-forward is the default proposal. Discard a candidate only through the user's explicit decision.

2. **Final Minutes.** Compile self-contained Final Minutes under [Section 5](#5-meeting-artifacts) after completing the approved actions in [Section 4](#4-post-meeting-actions).
   Preserve essential constraints and supported outcomes.
   Include the intended Handoff Plan.
   Identify material gaps without speculation.
   Later Execution reads Final Minutes for applicable instructions without requiring access to the internal live Working Record.

3. **Closing order.** Complete substantive closing work and required artifact checks before finalizing closure. Record the actual Closing Time consistently in Minutes and the Working Record.

   Use the user's applicable local:

   - Date.
   - Time.
   - Timezone.

   Preserve closed Meeting records and Minutes as immutable records.

4. **Indexed closure.** When Database indexing is enabled, update these fields of the existing Meeting together:

   - Status.
   - Closing metadata.
   - Final Minutes source.

   Preserve unrelated metadata and the Working Record reference. Verify the resulting state before claiming closure.

5. **Future Meeting Topics.** After verified closure, register confirmed carry-forward topics in the owning Identity Context Future Topics Chapter.

   Each entry needs:

   - A Topic Name.
   - A short Description.
   - A precise source reference.

   Keep one readable list. Exclude:

   - Independent topic statuses.
   - Counters.
   - Removal history.

6. **Meeting Plans.** A Meeting Plan remains provisional future work until the user adopts it. Plans and carry-forwards do not automatically open Meetings or authorize Jobs.

7. **Final Handoff.** Identify authorized recipients and authoritative sources before closure.
   Distinguish sources for reading from authorized writing destinations.

   Complete the following after verified Meeting closure:

   1. Update Identity Context and Future Topics.
   2. Consolidate qualifying Knowledge Base content under [Foundation Section 4](01-foundation.md#4-scoped-knowledge-base).
   3. Perform full-lifecycle Experience Capture.
   4. Send the authorized Handoff last.

   Each recipient applies its own Role Lifecycle, Scope selection and approval gates.
   Use Manual Handoff under [Records, Messaging and Experiences Section 2.6](05-records-messaging-and-experiences.md#2-messaging) when Messaging is unavailable.

## 4. Post-Meeting Actions

1. **Own operating resources.** Meeting Identities maintain their own Context and current Working Records within governing rules.
   They may maintain applicable shared Knowledge Bases within their Responsibility and Scope.
   Identity Context maintenance follows [Foundation Section 3](01-foundation.md#3-identity-context).
   Knowledge Base maintenance follows [Foundation Section 4](01-foundation.md#4-scoped-knowledge-base).

2. **Other Deliverables.** Before editing other Deliverables or files, the Meeting Identity must obtain approval for the relevant Scope.
   Authority depends on Responsibility and approval, regardless of amendment size or file type.
   The Meeting Identity owns its approved Post-Meeting Actions and resulting Deliverables.

3. **Closing transition.** CLOSE MEETING initiates Closing and normal approved Post-Meeting Action execution.
   Finish every approved, Meeting-Agent-owned Post-Meeting Action before compiling Final Minutes.
   Preserve each action's actual outcome in the Working Record.
   Other Identities' work remains a separate authorized Handoff.
   Post-closure Knowledge Base consolidation follows [Foundation Section 4.8](01-foundation.md#4-scoped-knowledge-base).
   Apply the finalized record requirements in [Section 3.3](#3-closing-and-handoff).

4. **Immediate execution.** Before Closing, execute an identified action only when the user expressly authorizes immediate execution.

   Discussion or confirmation of a required action alone does not authorize immediate execution.

## 5. Meeting artifacts

1. **Separate purposes.** Every Meeting must have an internal Working Record and separate user-facing Final Minutes.
   The Working Record supports durable Agent continuity.
   Final Minutes provide a consolidated, independently readable account.

2. **Shared metadata.** Both artifacts must identify:

   - Meeting ID.
   - Identity.
   - Role.
   - Topic.
   - Focus.
   - Expected Outcome.
   - Status.
   - Opening Time.
   - Closing Time.

3. **Working Record.** The append-oriented Working Record must primarily follow the confirmed Agenda.
   It must have five functional Chapters:

   1. Meeting Information.
   2. Confirmed Agenda.
   3. Agenda Outcomes.
   4. Post-Meeting Action Log.
   5. Authoritative Sources.

   Preserve accepted outcomes under [Section 2](#2-discussion-and-outcomes) rather than a conversation transcript.
   Persistence follows [Section 2.4](#2-discussion-and-outcomes).

4. **Final Minutes.** Final Minutes must have five Chapters:

   1. Meeting Information & Agenda.
   2. Confirmed Findings & Decisions.
   3. Actions & Outcomes.
   4. Open Matters & Dispositions.
   5. Sources & Quality Verification.

   Findings and Decisions share one substantive Chapter.
   Preserve their respective meaning under [Section 2.3](#2-discussion-and-outcomes).
   Final Minutes must satisfy [Global Writing Requirements](global-writing-requirements.md) and full Content, Writing and Formatting verification under [Quality Section 1](06-quality.md#1-deliverable-quality-and-independent-qa).

5. **Minutes organization.** The Meeting Agent determines the internal subject grouping, heading hierarchy, order and presentation.
   Organize Final Minutes by related subject matter without requiring Agenda chronology.
   Related outcomes from different Agenda items may be consolidated.
   Preserve the full adopted substance.
