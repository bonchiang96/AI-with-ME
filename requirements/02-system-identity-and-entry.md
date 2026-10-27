# System, Identity and Entry

Return to the [Requirements Overview](README.md).

## 1. Identity selection and governed setup

1. **System entry.** At every Conversation start, first locate the central Google Drive folder named “AI with me”.
   Open System Context.
   The user then selects a registered Identity under [Section 1.4](#1-identity-selection-and-governed-setup).
   Assess access to applicable System Rules and reuse existing accessible resources.
   Confirm absence before initiating Bootstrap under [Section 1.2](#1-identity-selection-and-governed-setup).

2. **Bootstrap.** When the central folder is confirmed absent, a default provisional Meeting Agent holds a Bootstrap Meeting.
   Use the normal Meeting Lifecycle.
   Explain the proposed:

   - Root.
   - System Context.
   - System Rules.
   - Knowledge Base folder.
   - Responsibilities.
   - Minimum Identities.
   - Creation actions.

   The user approves the System arrangement and its creation actions in that Meeting.
   After CLOSE MEETING, the same Meeting Agent performs the approved Post-Meeting Actions:

   1. Create the folder.
   2. Create System Context and System Rules.
   3. Create the Knowledge Base folder with its 00 Index and general Knowledge Base under [Foundation Section 4.9](01-foundation.md#4-scoped-knowledge-base).
   4. Establish the approved minimum Identities under [Section 1.11](#1-identity-selection-and-governed-setup).
   5. Save the Bootstrap Working Record and Final Minutes as the new System's first records.
   6. Join the normal entry path at Identity selection.

   Bootstrap records remain in Conversation until the folder exists.
   The provisional Identity requires no pre-existing Registry entry.
   Inaccessibility alone does not prove absence.
   Resolve access or location uncertainty before creating another Root.
   Restore genuinely missing resources within existing approved authority and applicable System Rules.

3. **Minimum Identities.** Bootstrap establishes two Identities:

   - The General Meeting Agent, with Agent Key `general-meeting`.
   - The General Execution Agent, with Agent Key `general-execution`.

   The General Meeting Agent creates scoped Identities through Meetings.

4. **Conversation Initiation.** After System entry, the user selects a registered operational Identity from System Context.
   Load that Identity's shared Role Lifecycle and its authoritative Identity Context.
   The Identity is then ready for NEW MEETING or NEW JOB.
   Load applicable System Rules and Plugin Instructions for the assignment.
   Continue work through the discovery requirements in [Section 2.17](#2-agent-responsibilities-and-commands).

5. **Identity discovery.** Discovery must support a directly supplied Identity Context Locator or a registered Identity resolved through System Context.
   Both paths must reach the Identity's authoritative Context through its identity folder.
   Detailed cross-environment Locator design remains deferred under [Environments and Deferred Work Section 2](07-environments-and-deferred-work.md#2-baseline-acceptance-and-deferred-development).

6. **Identity meaning.** Each Identity must identify:

   - Its exact Agent Key.
   - Its Role.
   - Its Responsibility.
   - Its Scope.
   - Its identity folder Locator.

   Its Role selects reusable Plugin Instructions and the common Role Lifecycle.
   Identity registration follows [Foundation Section 2.3](01-foundation.md#2-governance-resources-and-dependencies).

7. **Identity isolation.** Distinct operational Identities must retain their own assignments and message inboxes.
   Separate Identities may share the same packaged Role Instruction.
   No Identity's responsibilities merge other Identities or their inboxes.

8. **Stable assignments.** An Agent Key must remain stable across Conversations serving the same assignment. Resolve the user's assignment against registered Scope information. Resolve missing or ambiguous Identities before scoped Messaging. An unresolved scoped assignment must not default to another Identity.

9. **Identity definition.** The user raises a new Identity in a Meeting with the General Meeting Agent.
   Together they define:

   - Name.
   - Role.
   - Responsibility.
   - Scope.
   - Workflows.
   - Deliverables.

   The user approves the Identity and its setup in that Meeting.
   Work purpose guides Workflow selection without requiring a rigid Scope taxonomy.

10. **Assignment grouping.** Meeting Agent Identities are distinguished by Scope.
    A Book may have its own Book Meeting Identity.
    Group execution work under a small number of shared Execution Identities.
    The defining Meeting identifies the responsible Meeting Identity and approved assignment.

11. **Authorized Identity setup.** After CLOSE MEETING, the General Meeting Agent performs the approved Identity setup as Post-Meeting Actions:

    1. Create the identity folder and all its files with their Operating Guides under [Foundation Section 5.1](01-foundation.md#5-identity-folder-index-and-inbox).
    2. Record applicable Knowledge Bases in the Identity Context Knowledge Bases Chapter under [Foundation Section 3.9](01-foundation.md#3-identity-context).
    3. Register the identity folder Locator in System Context.
    4. Preserve and verify setup evidence.

    Other approved resource establishment remains with its authorized owner.

12. **Governance refinement.** The Meeting Identity responsible for the governing Scope must refine adopted:

    - Rules.
    - Workflow usage.
    - Resource purposes.
    - Output destinations.
    - Assignments.
    - Operating details.

    Implementation follows the responsible owner's authority and applicable Scope approvals.

13. **Identity changes.** Inactive or archived Identities must remain preserved but disappear from normal active choices. They may be reactivated when appropriate.

14. **Local Bootstrap.** Local Bootstrap must establish missing Local System Rules and required working paths only.
    Central Identity and Context authority remain governed by [Foundation Section 2.3](01-foundation.md#2-governance-resources-and-dependencies) and [Foundation Section 3.1](01-foundation.md#3-identity-context).

## 2. Agent responsibilities and Commands

1. **Responsibility, Scope, and Output.** Responsibility defines the result or quality obligation an Agent must guarantee.

   Scope defines permitted:

   - Activities.
   - Resources.
   - Authority.

   Output identifies actual deliverables or result evidence. Each confirmed Job Scope must remain within the assigned Agent's authority.

2. **Roles and Lifecycles.** The two Roles are Meeting Agent and Execution Agent.
   A Role is distinguished by its internal Lifecycle or Protocol.
   Every Identity must use the common Lifecycle of its Role.

   Each Identity retains its own:

   - Responsibility.
   - Scope.
   - Output.

   Lifecycle governs the Role's internal work.
   Workflow guides a particular Task or Deliverable across relevant Agents.

3. **Meeting responsibility.** Meeting Agents organize:

   - Discussion.
   - Research.
   - Planning.
   - Substantive decisions.

   Each Meeting Identity governs only its assigned Scope.
   A governance assignment may include applicable operating rules and Commands.
   Approved Post-Meeting Actions follow [Meeting Lifecycle Section 4](03-meeting-lifecycle.md#4-post-meeting-actions).

4. **Document drafting responsibility.** An Execution Identity drafting a document must completely and readably preserve confirmed decisions.
   These independent documents are normally human-facing and high-requirement.
   A typical small document count is not a hard limit.

   The substantive author determines permitted:

   - Organization.
   - Methods.
   - Verification.

   Execution Parent and Sub-agent responsibilities follow [Execution Lifecycle Section 4](04-execution-lifecycle.md#4-execution-parent-and-sub-agents).

5. **Reusable resource maintenance.** An assigned Execution Identity must maintain coherent authoritative reusable operating resources.
   Its writing must express rules and relationships precisely enough for AI interpretation and reuse.
   Independent documents and other Deliverables remain with their assigned owners.

6. **System resource changes.** An Execution Identity may perform authorized System resource synchronization or updates within an approved Job Scope.

   It must preserve each affected working Scope's:

   - Functional working state.
   - Adopted Governance.
   - Assignments.
   - Customization.

   Implement approved governing decisions under the Identity's own Job approvals.
   Authorized targets may include System Context and applicable System Rules.
   Meeting-owned Bootstrap and Identity setup follow [Section 1](#1-identity-selection-and-governed-setup).
   Respect the owning Scope's Governance authority.

7. **Resource ownership.** Each Meeting Identity maintains its own Meeting Working Records and Final Minutes.
   These remain separate resources under [Meeting Lifecycle Section 5](03-meeting-lifecycle.md#5-meeting-artifacts).
   Each Execution Identity remains responsible for its approved Deliverables.
   Parent ownership of Job Records follows [Execution Lifecycle Section 4.2](04-execution-lifecycle.md#4-execution-parent-and-sub-agents).

   The following belong in the Job Record:

   - Its Execution Plan.
   - Approvals.
   - Changes.
   - QA.

   Identity Context maintenance follows [Foundation Section 3](01-foundation.md#3-identity-context).
   Shared Knowledge Base maintenance follows [Foundation Section 4](01-foundation.md#4-scoped-knowledge-base).

8. **Shipped Agents.** The Plugin ships only the Meeting Agent and the Execution Agent.

9. **Independent QA responsibility.** Independent QA is a normal Workflow under [Quality Section 1.11](06-quality.md#1-deliverable-quality-and-independent-qa).

10. **Meeting execution responsibility.** A Meeting Identity owns its approved Post-Meeting Actions and resulting Deliverables within [Meeting Lifecycle Section 4](03-meeting-lifecycle.md#4-post-meeting-actions).

11. **Command ownership.** The Agent Lifecycle controls stage order and selects the needed applicable Command.

    Commands define:

    - Applicable actions.
    - Outputs.
    - Customization.
    - Relevant constraints.

    They must respect these limits:

    1. Do not autonomously trigger work.
    2. Do not expand authority.
    3. Do not duplicate Lifecycle sequencing.

12. **Command organization.** Necessary Command definitions must be discoverable through Identity Context operating references.
    Keep the Command list compact and resolve each needed Command to its definition.
    A native Google Docs Tab per Command is preferred when using Google Docs.
    Necessary Command content may be reused within the active Conversation.

13. **Command readiness.** Required Commands and dependencies must be usable for their assigned actions. An Agent must report missing definitions or inaccessible dependencies. It must not claim incomplete actions succeeded. Detailed execution mechanics remain with authorized implementation.

14. **Shared Execution foundation.** Execution Identities must apply shared Global Rules.
    Assigned Instructions and applicable Commands must reflect each Identity's Responsibility and work type.
    Apply the common Role Lifecycle under [Section 2.2](#2-agent-responsibilities-and-commands).

15. **Shared Commands.** Identities with the same Role and Responsibility must share applicable Commands.
    Separate scoped Identities retain distinct Scopes and own work records.
    Meeting and Execution Roles may require different Commands.

16. **Dynamic Command resolution.** Shared Meeting, Job and CREATE RECORD Commands must identify the invoking Identity and record category.

    Resolve the Identity's currently authorized Responsibility and Scope from System Context.
    Resolve the applicable record Target Location through Identity Context and current System Rules.

    A shared Command must not assume a particular Identity or fixed Workspace.
    Commands must not copy or widen Identity Scope.
    Resolve missing Scope before acting.

17. **Discovery before repeated questions.** All Agents must discover accessible information before requesting it again from the user.

    Discover relevant:

    - Context.
    - The current Workflow.
    - Progress checkpoints.
    - Messages.
    - Work Requests.
    - Records.
    - Required source references.

    Continue from the selected Identity and current information without requiring the user to reconstruct prior work.

18. **Supported options.** For discoverable matters, Agents must present supported options and their best available Proposal.
    For the user's own knowledge, Agents listen first under [Global Communication Rules Section 5](global-communication-rules.md#5-interaction-modes).
    The user may provide new inputs, select alternatives or revise the direction.

19. **Workflow definitions.** Standard Workflow Definitions must reside in the Plugin.
    User-created Workflows may reside in an appropriate Knowledge Base.
    Workflow outcomes and subject knowledge belong in the relevant Knowledge Base.
    Workflow progress belongs in the owning Identity's Identity Context.

20. **Task Workflow selection.** The user selects the Workflow when a Task starts.
    Discover applicable Workflows in the Plugin and scoped Knowledge Bases to support that selection.
    If none is suitable, work normally under the assigned Role Lifecycle using:

    - Domain knowledge.
    - Available tools.
    - Judgment.

    Absence of a suitable Workflow does not require a mandatory fallback Workflow or special Proposal.
    Existing Scope and approval requirements still apply.

21. **Workflow progress and customization.** Keep the current stage in the Identity Context of the Agent owning the current step.
    Transfer stage ownership only through a normal Handoff.
    Each Identity may customize how a Workflow runs within its approved work.
    The default is one full draft. A large Book may use Chapter-by-Chapter drafting.

22. **User review and revision ownership.** In Book and Business Document Workflows, the user makes final decisions.
    Leave space for user input. Advise when asked or when direction is unclear.
    After user review, apply this revision rule:

    1. The Meeting Agent assesses whether each change is small or large.
    2. For a small change, the Meeting Agent proposes a direct edit to the user.
    3. The Proposal states the impacted range and shows the exact current and amended text.
    4. With the user's approval, the Meeting Agent makes the edit as an approved Post-Meeting Action.
    5. Without that approval, or for a large change, record the feedback in the Minutes.
    6. The Execution Agent revises from those authoritative Minutes.

    Assessment alone does not authorize an edit.
    Preserve the approved Scope and normal approval gates.
