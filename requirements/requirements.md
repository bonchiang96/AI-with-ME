# AI with ME - Operating Framework

## 1. Purpose and interpretation

### 1.1 Framework definition

1. **Framework identity.** The name “AI with ME - Operating Framework” covers:

   - The Plugin.
   - Google governance resources.
   - Their operating relationships.
   - Optional supporting Database services.

   It is a portable AI Operating Framework across supported environments.

2. **Core purpose.** The Framework's core purpose is knowledge transfer.
   AI helps users express their knowledge accurately in written form.
   Other AI Agents and people must be able to read and understand that knowledge.

   Support reusable, portable work with:

   - Clear responsibility.
   - Bounded Scope.
   - User decisions.
   - Durable authoritative records.

   It should reduce unnecessary source reads and duplicated instructions.

3. **Meaning of requirements.** Interpret these requirement terms consistently:

   1. “Must” states a required outcome.
   2. “Should” preserves an intended preference.
   3. “May” identifies permitted flexibility.

   Conditions and qualifications remain part of each requirement.

4. **Substantive authority.** The user remains the final decision-maker. Confirmed governing decisions establish substantive requirements.

   The following do not independently authorize execution:

   - Messages.
   - Proposals.
   - Accepted Findings.
   - Advisory Experiences.

5. **Interaction modes.** Choose the interaction mode according to the situation:

   1. For discoverable matters, discover accessible information and present a supported Proposal.
      Examples include Meeting preparation, Handoff recipients and Knowledge Base selection.
   2. For the user's own knowledge, listen first and restate your understanding.
      The user confirms or corrects it. Leave Agenda space for user input.
   3. For document review, first perform an independent AI review.
      Cover fidelity, Writing Requirements and presentation style.
      Then provide separate Agenda space for the user's review. Consolidate both reviews.

   Accurate confirmation must preserve the user's intended knowledge.

### 1.2 Binding Non-functional Requirements

These Non-functional Requirements bind relevant design and maintenance of:

- Requirements.
- The AI Plugin.
- Agent Instructions.
- Lifecycles.
- Workflows.

1. **AI Management.** The Framework governs AI Management. Keep it distinct from Software Management, whose design principles and expectations differ.

2. **AI autonomy.** The Framework defines:

   - Source authority.
   - Agent responsibilities.
   - Scope.
   - Dependencies.
   - Forward Lifecycles.
   - Workflows.
   - Required approvals.
   - Expected outcomes.

   The executing AI selects practical methods within these requirements and its available capabilities. It solves operational problems using its own judgment.

   Agent Lifecycles must preserve:

   - Essential stages.
   - Decisions.
   - Information handling.
   - Handoffs.

3. **Priorities and boundaries.** Define meaningful priorities and essential Scope boundaries.
   Settle forward-flow requirements under Section 1.2.8.
   Allow reasonable ambiguity in implementation methods without leaving incompatible forward flows unresolved.

   Do not specify every possible:

   - Edge case.
   - Condition.
   - Micro-boundary.

4. **Failure Handling.** AI must use its judgment when execution encounters difficulties. It must act within authorized Scope and record actual outcomes. Report necessary assistance.

   Do not predesign Failure Handling methods for the AI.

   Normal AI execution must not require:

   - Fixed retry counts.
   - Exhaustive recovery branches.

   Delegated acceptance review follows Section 7.4.

5. **AI behavior verification.** Individual AI behavior and choices may vary between executions.

   Do not require:

   - Deterministic, repeatable verification of individual AI behavior.
   - A universal AI-response Verification stage.

   Actual Deliverable QA follows Section 9.

6. **Writing, design and operating preferences.** Preserve the following as binding Non-functional Requirements:

   - AI-native constraints.
   - Writing and design principles.
   - Relevant user operating preferences.

   Apply the writing and user communication requirements in Section 9.

7. **Requirement numbering.** Use the document's Section numbering to locate requirements. Do not add parallel R-prefixed identifiers to every requirement.

8. **Forward-flow completeness.** Requirements must settle every item that determines:

   - Step order.
   - The responsible owner.
   - The approver.
   - Resources read.
   - Resources written.
   - The outcome.

   An item belongs in Requirements when two developers could otherwise implement incompatible flows.
   Implementation design may remain deferred only when the required outcome is stated.
   Detailed design boundaries follow Section 12.5.

## 2. Repository, distribution, and installation

1. **Source authority.** One GitHub Repository must be the authoritative development and distribution source for the Plugin and reusable operating resources. Maintain their common instructions in that source.

2. **README.** The root README must explain the Framework for its readers in plain words.
   Use Global Writing Requirements Standard Mode.

   Include:

   - What the Framework is and why it exists.
   - One simple flow picture.
   - Required and optional dependencies.
   - A short getting-started placeholder.
   - Resource locations.
   - The License.

   Link to the Requirements instead of restating their rules.
   Direct readers to available resources and identify future resources accurately.
   Neither the Requirements nor README carries version labels.
   GitHub commit history provides versioning.

3. **Requirements area.** A dedicated Requirements area must contain the consolidated requirements baseline. Source-to-requirement traceability must remain durable. Private governance references belong in private supporting records.

4. **Plugin area.** A separate Plugin area must contain:

   - Plugin source.
   - Packaged resources.
   - The eventual installable deliverable.

   It must provide these reusable resources:

   - Agent Instructions.
   - Initiation.
   - Forward Lifecycles.
   - Applicable Frameworks.

5. **Documentation area.** A separate, richer Documentation area is a desired reference.

   It should explain:

   - Concepts.
   - Principles.
   - Operation.
   - Environments.
   - Integration expectations.
   - Detailed usage.

   Its practical organization belongs to authorized drafting work.

6. **Private installation.** Distribution must support users performing these actions with their own Private Plugin from GitHub source:

   - Creating it.
   - Manually installing it.
   - Manually updating it.

   Packaging and update methods remain subjects for authorized development.

7. **AI-led installation.** A user may give an AI the Repository URL.

   The AI must complete these actions:

   1. Read the README.
   2. Locate the Plugin and installation guidance.
   3. Assess dependencies.
   4. Assist installation using available tools and granted permissions.

8. **Missing capabilities.** The AI must explain the practical limitation when any necessary dependency is unavailable:

   - A connector.
   - A capability.
   - A permission.

   It must discuss the next authorized step. It must perform or guide permitted setup within its capabilities.

9. **Installed operation.** The installed Plugin must contain shared instructions and resources required for normal Agent operation without routine GitHub reads. GitHub supplies intentional updates and source distribution. Current governance and records must be obtained from their Google authority.

10. **Installation design boundary.** AI-native installation guidance is required. Public Plugin publication and automatic GitHub synchronization are outside the adopted distribution design.

    The following are not mandatory requirements:

    - Compatibility matrices.
    - Per-AI packages.
    - Platform installation tests.

11. **External setup guidance.** Framework GitHub documentation must describe AI with ME rather than store fixed third-party setup steps.
    If Supabase is selected, research current official setup instructions when guidance is actually needed.

## 3. Resources, dependencies, and rule authority

### 3.1 Governance resources and dependencies

1. **Google authority.** Google Drive / Docs must provide the main authoritative document environment for governance and required records.

   This authority applies across:

   - ChatGPT.
   - Local environments.
   - Future independent AI execution.

2. **System Root.** The central Google Drive System Root must be named “AI with me”.
   It must provide access to:

   - Central System Context.
   - Applicable System Rules.
   - Resources for registered working Scopes.

   Environment System Rules govern their actual storage structure.
   Local environments must use this central Root rather than create another System Root.
   Bootstrap follows Section 4.2.

3. **System Context.** Google System Context must provide central authority for Identity registration and Identity Context information.
   Its Registry must contain:

   - Identities.
   - Knowledge Bases.

   Each registered Identity must have an exact Identity Context Locator.
   Maintain one authoritative registration per Identity, including its assigned Responsibility and Scope.
   Local environments must use the assigned central Identity without creating a separate Local Identity Registry.

   Preserve current System configuration and appropriate optional Database connection references.
   Routine progress belongs in its owning records or current Identity references.

4. **System Rules.** System Rules must express user-defined shared operating conventions.
   Google System Rules must govern Google-side:

   - Document creation.
   - Locations and storage structure.
   - Resource maintenance.
   - Optional Database enablement.

   Local System Rules must govern:

   - Local file formats.
   - Naming.
   - Directories and working paths.
   - Local Record creation.
   - Local Deliverable creation.
   - Which outputs synchronize to Google.
   - Applicable optional Database usage.

   Applicable environment System Rules must govern synchronization and Database Atomic Action order and timing.
   Apply the rules for the actual execution environment.
   Rule priority follows Section 3.1.8.

5. **Resource purposes and destinations.** Governing configuration must define known deliverables and meaningful destinations.
   For each maintained resource, identify the necessary:

   - Purpose.
   - Expected outcome.
   - Location.
   - Responsible Identity.

   Identity Context must reference its own applicable record destinations under Section 3.2.3.
   Storage follows Section 3.1.4.

6. **Workflow customization.** Governed working arrangements may customize a Workflow's:

   - Stage outcomes.
   - Deliverables.
   - Target Locations.
   - Assigned maintenance responsibilities.

   These arrangements may evolve through confirmed decisions and practical work.
   Preserve Role Lifecycle authority under Section 5.2.

7. **Context discovery.** An Identity must open its own Identity Context to discover relevant:

   - Records.
   - Collaboration partners.
   - Deliverables.
   - Working references.

   System Context supplies the registered Identity Context Locator.

8. **Contextual priority.** Applicable System Rules override conflicting Plugin instructions for the environment operations in Section 3.1.4.

   Interpret other governing overlap using:

   - Context.
   - Purpose.
   - Source authority.
   - Known intent.
   - The situation.

   An exhaustive override matrix or mechanical conflict algorithm is not required.

9. **Source loading.** Agents should reuse static instructions available in the effective Conversation Context unless their applicability changes.
   They must read dynamic context and working data when current information is needed.
   Load applicable Commands selectively at the relevant Lifecycle stage.
   Local Agents need not reread Google for each ordinary file operation.

10. **Meaningful resources.** Every maintained resource should serve an identified purpose. Resource creation must follow authorized Responsibility, Scope and actual operating needs.

11. **Optional Database.** Database services are optional.

    They may support:

    - Indexes.
    - Search.
    - Agent Messaging.
    - Handoff.
    - Other approved capabilities.

    Common usage guidance belongs in the Plugin.
    Configuration and suitable connection references belong in System Context.
    Applicable System Rules govern service enablement.
    Credential and configuration-template details require later authorized design.

12. **Database-free operation.** Without Database services, Agents must omit unavailable Database-dependent operations. Apply the manual handoff requirements in Section 8. Identity discovery and essential governance must remain possible through Google resources.

13. **Integration expression.** Integration requirements must identify:

    - The authoritative resource.
    - The necessary action.
    - The expected output.
    - Applicable constraints.

    Database RPC descriptions need authoritative function names and defined inputs and outputs. Connector invocation methods belong to the executing AI.

14. **Directory references.** Each resource reference requires only:

    - A useful Title.
    - A useful Description.
    - A useful Locator.

    Add fields only when they serve a genuine directory purpose. Keep each directory compact. Identity Context current references follow Section 3.2.

### 3.2 Identity Context

1. **Starting context.** Every Identity must maintain one consolidated central Google Identity Context as its starting context for work.
   It contains current working information, future work and operating references.
   It is not described as memory.
   Complete historical evidence belongs in its original Records and Minutes.
   Local environments use this authoritative Context without creating a duplicate Local Context.

2. **Required Chapters.** Identity Context must contain these six Chapters:

   1. Context Management Rules.
   2. Future Topics.
   3. Working Group.
   4. Important Learning.
   5. Important Things or High-Priority Items.
   6. Deliverable Index.

   Working Group contains peer Identities and Handoff relationships.
   Deliverable Index contains the latest authoritative Deliverable locations and present condition.

3. **Own record locations.** Identity Context must reference applicable Target Locations for its own:

   - Minutes.
   - Working Records.
   - Job Records.
   - Additional Identity-owned records or resources.

   Distinguish sources for reading from authorized record-writing destinations.

4. **Verified operating information.** An Identity may update its independently derived information whenever useful within its Responsibility and Scope.
   Its Deliverable Index may reflect relevant verified Deliverables whenever they become known, without awaiting Minutes.
   Register accepted and saved Deliverables under Section 7.2.6.
   The creating Execution Identity may update its Context Index immediately or consolidate updates at Job close.
   A Meeting Identity may refresh its relevant Index after receiving a Completion Notice at a later Meeting.

5. **User-originated decisions.** User-originated decisions require appropriate authoritative support.
   User-confirmed Meeting matters enter authoritative Identity Context only after verified Closed Meeting Minutes.
   Preserve the relevant source reference.

6. **Working Group.** Working Group may retain real collaboration selected by relevant participants.
   It may include useful Identity pairings and collaboration patterns.
   The Agent determines useful maintenance timing through judgment.
   User-originated decisions follow Section 3.2.5.

7. **Selected current references.** Identity Context may preserve useful:

   - Workflow references.
   - Useful Workflow usage.
   - The current Workflow stage.
   - Related Minutes.
   - Meaningful verified accomplishments.

8. **Organization.** Each Identity controls content organization within the six required Chapters.
   Keep each Chapter's meaning within its purpose.

### 3.3 Scoped Knowledge Base

1. **Knowledge resources.** A Knowledge Base must store external subject information for a defined Scope.
   Examples include:

   - A company.
   - A Brand.
   - A specialist domain.

   One Scope may contain multiple Knowledge Bases.
   Multiple Identities may use or maintain the same Knowledge Base.
   Register each Knowledge Base in System Context.
   Any Identity may maintain a corresponding System Context Registry entry when it performs either action:

   - Creates the Knowledge Base.
   - Changes the Knowledge Base's Scope or Topic.

2. **Current content.** Include only currently valid content within the Knowledge Base's Scope:

   - Confirmed external subject knowledge.
   - User-created Workflows permitted under Section 5.19.

   Preserve adopted future directions as future directions rather than completed implementation.

   Exclude:

   - Exploratory ideas.
   - Unresolved choices.
   - Superseded content.
   - Future Jobs.
   - Deliverable progress.

   Historical Closed Minutes and Records preserve past evidence.

3. **Decision classification.** After every Meeting closes with verified Closed Minutes, review the entire Minutes. Classify confirmed Meeting outcomes, including each Decision, by their actual meaning.

   One Decision may contain:

   - External subject knowledge.
   - Governance configuration.
   - Execution instructions.

   Route each part to its accountable owner without losing material meaning.

4. **Semantic routing.** Route confirmed meaning according to its owner:

   1. External subject knowledge belongs in an applicable scoped Knowledge Base.
   2. Identity operating information belongs in Identity Context under Section 3.2.
   3. Governance belongs in its applicable authoritative resources.
   4. Job-specific instructions remain in relevant Closed Minutes and Job authority.

   Mentioning a working Scope does not itself make an instruction subject knowledge.

5. **Consolidation.** For an update, read the complete current Knowledge Base.
   For Closed-Minutes-based consolidation, also read the new relevant verified Closed Minutes.
   Consolidate current scoped subject knowledge throughout the complete resource.
   Ordinary updates do not require rereading the full Historical Minutes collection.

   During consolidation:

   1. Retain all valid knowledge.
   2. Integrate newly confirmed subject matter.
   3. Replace only genuinely superseded content.
   4. Apply Global Writing Requirements Standard Mode.
   5. Useful paragraph-level source references may be included.

6. **Execution sources.** Execution must use relevant scoped Knowledge Bases for current subject knowledge. It must also use the specific authoritative Closed Minutes for work instructions. Execution completion alone does not trigger Knowledge Base maintenance.

7. **Maintenance triggers.** Apply these two distinct triggers within the Knowledge Base's Scope:

   1. An Agent may maintain independently discovered, sufficiently verified subject knowledge whenever useful.
      This maintenance is discretionary.
   2. Qualifying user-confirmed Topic or Scope knowledge must be consolidated from verified Closed Minutes after the Meeting closes.
      This maintenance is mandatory when qualifying content exists.

8. **Post-closure maintenance.** Closed-Minutes-based consolidation is routine post-closure maintenance rather than a pre-Minutes Post-Meeting Action.
   Save and verify its result independently.
   It must not reopen or modify immutable Minutes.

### 3.4 PROFIT + A Framework

1. **Framework purpose.** PROFIT + A must provide a reusable Framework for defining AI tasks and Prompts.
   PROFIT defines the task. A defines the readiness handshake before execution.

2. **Prompt applicability.** All Sub-agent Prompts and future Plugin Development Prompts must use the complete PROFIT + A Framework.
   Apply Strict Mode under Section 9.9.

3. **PROFIT elements.** Define these six elements for the task:

   1. **P — Persona.** Define who the AI should be for the task, including the necessary:
      - Role.
      - Skills.
      - Experience.
      - Domain knowledge.
   2. **R — Result.** Define the exact deliverable or outcome the AI should produce.
   3. **O — Objective.** Define why the task is necessary and what the Result should achieve.
   4. **F — Feed.** Identify the source material the AI receives to perform the task.
      Feed is the material itself. It may include:
      - Data.
      - Documents.
      - Images.
      - References.
      - Product information.
      - Previous outputs.
      - Other inputs.
   5. **I — Insight.** Define how the Feed should be understood and how the Result should be shaped.
      Insight may include:
      - Audience.
      - Platform.
      - Tone.
      - Constraints.
      - Priorities.
      - Research findings.
      - Strategic direction.
      - Other interpretation.
   6. **T — Template.** Define the final Result's:
      - Structure.
      - Format.
      - Presentation.

4. **Feed Modes.** Use the applicable mode:

   1. **Provide Now.** Include the required Feed with the Prompt.
   2. **Provide Later.** Define the required Feed. The user provides it in the next message.
   3. **Continuous Feed.** Continue the task across multiple turns.
      New Feed may affect earlier working context through:
      - Additions.
      - Changes.
      - Replacement.

5. **Acknowledgement.** Acknowledgement must remain the final part of the Prompt.
   Apply the readiness handshake for the selected Feed Mode:

   1. **Provide Now.** The AI confirms readiness. It waits for the user's explicit start signal before execution.
   2. **Provide Later.** The AI performs these steps:
      1. Confirm readiness.
      2. State the required Feed.
      3. Execute once that Feed is provided.
   3. **Continuous Feed.** The AI confirms readiness once at the start or reset point.
      It then processes subsequent Feed directly.

6. **Feed In.** Feed In is a supporting concept, separate from PROFIT + A.
   It defines what the user needs to prepare or provide to use the Prompt.

7. **Prompt composition.** Arrange the six PROFIT elements in any order that makes the final Prompt clear and natural.
   In the final Prompt:

   - I refers to the user.
   - You refers to the AI.

   During Framework review or drafting, describe definitions naturally.
   Do not force I / You wording before composing the final Prompt.

## 4. Identity selection and governed setup

1. **System entry.** At every Conversation start, first locate the central Google Drive folder named “AI with me”.
   Open System Context.
   The user then selects a registered Identity under Section 4.4.
   Assess access to applicable System Rules and reuse existing accessible resources.
   Confirm absence before initiating Bootstrap under Section 4.2.

2. **Bootstrap.** When the central folder is confirmed absent, a default provisional Meeting Agent holds a Bootstrap Meeting.
   Use the normal Meeting Lifecycle.
   Explain the proposed:

   - Root.
   - System Context.
   - System Rules.
   - Responsibilities.
   - Minimum Identities.
   - Creation actions.

   The user approves the System arrangement and its creation actions in that Meeting.
   After CLOSE MEETING, the same Meeting Agent performs the approved Post-Meeting Actions:

   1. Create the folder.
   2. Create System Context and System Rules.
   3. Register the approved minimum Identities.
   4. Save the Bootstrap Working Record and Final Minutes as the new System's first records.
   5. Join the normal entry path at Identity selection.

   Bootstrap records remain in Conversation until the folder exists.
   The provisional Identity requires no pre-existing Registry entry.
   Optional Database services may be discussed during Bootstrap.
   Inaccessibility alone does not prove absence.
   Resolve access or location uncertainty before creating another Root.
   Restore genuinely missing resources within existing approved authority and applicable System Rules.

3. **Minimum identities.** A usable System must expose at least the System-wide Meeting Identity and an Execution Identity assigned System administration.

4. **Conversation Initiation.** After System entry, the user selects a registered operational Identity from System Context.
   Load that Identity's shared Role Lifecycle and its authoritative Identity Context.
   The Identity is then ready for NEW MEETING or NEW JOB.
   Load applicable System Rules and Plugin Instructions for the assignment.
   An unselected Identity must not automatically select System administration.
   Continue work through the discovery requirements in Section 5.17.

5. **Identity discovery.** Discovery must support a directly supplied Identity Context Locator or a registered Identity resolved through System Context.
   Both paths must reach the Identity's authoritative Context.
   Discovery must work independently of Database services.
   Detailed cross-environment Locator design remains deferred under Section 12.

6. **Identity meaning.** Each Identity must identify:

   - Its exact Agent Key.
   - Its Role.
   - Its Responsibility.
   - Its Scope.
   - Its Identity Context Locator.

   Its Role selects reusable Plugin Instructions and the common Role Lifecycle.
   Identity registration follows Section 3.1.3.

7. **Identity isolation.** Distinct operational Identities must retain their own assignments and message inboxes.
   Separate Identities may share the same packaged Role Instruction.
   System administration responsibilities do not merge other Identities or their inboxes.

8. **Stable assignments.** An Agent Key must remain stable across Conversations serving the same assignment. Resolve the user's assignment against registered scope information. Resolve missing or ambiguous identities before scoped Messaging. An unresolved scoped assignment must not default to another Identity.

9. **Identity definition.** The user raises a new Identity in a Meeting with the System-wide Meeting Agent.
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

11. **Authorized Identity setup.** After CLOSE MEETING, the System-wide Meeting Agent performs the approved Identity setup as Post-Meeting Actions:

    1. Create the Identity Context.
    2. Register the Identity in System Context.
    3. Preserve and verify setup evidence.

    Other approved resource establishment remains with its authorized owner.
    System administration responsibility follows Section 5.6.

12. **Governance refinement.** The Meeting Identity responsible for the governing Scope must refine adopted:

    - Rules.
    - Workflow usage.
    - Resource purposes.
    - Output destinations.
    - Assignments.
    - Operating details.

    Implementation follows the responsible owner's authority and applicable Scope approvals.

13. **Identity changes.** Inactive or archived identities must remain preserved but disappear from normal active choices. They may be reactivated when appropriate.

14. **Local Bootstrap.** Local Bootstrap must establish missing Local System Rules and required working paths only.
    Central Identity and Context authority remain governed by Sections 3.1.3 and 3.2.1.

## 5. Agent responsibilities and Commands

1. **Responsibility, Scope, and Output.** Responsibility defines the result or quality obligation an Agent must guarantee.

   Scope defines permitted:

   - Activities.
   - Resources.
   - Authority.

   Output identifies actual deliverables or result evidence. Each confirmed Job Scope must remain within the assigned Agent's authority.

2. **Roles and Lifecycles.** The two principal Roles are Meeting Agent and Execution Agent.
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
   Approved Post-Meeting Actions follow Section 6.4.

4. **Document drafting responsibility.** An Execution Identity assigned document drafting must completely and readably preserve confirmed decisions.
   These independent documents are normally human-facing and high-requirement.
   A typical small document count is not a hard limit.

   The substantive author determines permitted:

   - Organization.
   - Methods.
   - Verification.

   Execution Parent and Sub-agent responsibilities follow Section 7.4.

5. **Reusable resource maintenance.** An assigned Execution Identity must maintain coherent authoritative reusable operating resources.
   Its writing must express rules and relationships precisely enough for AI interpretation and reuse.
   Independent documents and other Deliverables remain with their assigned owners.

6. **System administration responsibility.** An assigned Execution Identity owns authorized:

   - System resource establishment.
   - Synchronization or updates.

   It must preserve each affected working Scope's:

   - Functional working state.
   - Adopted Governance.
   - Assignments.
   - Customization.

   Implement approved governing decisions under the Identity's own Job approvals.
   Authorized targets may include System Context and applicable System Rules.
   Meeting-owned Bootstrap and Identity setup follow Section 4.
   Respect the owning Scope's Governance authority.

7. **Resource ownership.** Each Meeting Identity maintains its own Meeting Working Records and Final Minutes.
   These remain separate resources under Section 6.5.
   Each Execution Identity remains responsible for its approved Deliverables.
   Parent ownership of Job Records follows Section 7.4.2.

   The following belong in the Job Record:

   - Its Execution Plan.
   - Approvals.
   - Changes.
   - QA.

   Identity Context maintenance follows Section 3.2.
   Shared Knowledge Base maintenance follows Section 3.3.

8. **Database Engineer responsibility.** An Execution Identity assigned Database Engineering owns the following within approved database work:

   - Infrastructure.
   - Implementation.
   - Integrity.
   - Operation.
   - Stability.
   - Compatible Contracts.

   It must inspect current state. It must verify actual behavior. Routine Agents use applicable interfaces directly within their authority.

9. **Independent QA responsibility.** One dedicated Execution Identity assigned Central QA must provide assessments and reports that are:

   - Independent.
   - Complete.
   - Objective.

   Its Jobs and reports remain under System-level authority.
   It may inspect other working Scopes only within specifically approved Job Scope.

   It must respect these limits:

   1. Do not edit inspected resources.
   2. Do not authorize remediation.
   3. Do not independently schedule audits.

10. **Meeting execution responsibility.** A Meeting Identity owns its approved Post-Meeting Actions and resulting Deliverables within Section 6.4.

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
    Keep the Command Index compact and resolve each needed Command to its definition.
    A native Google Docs Tab per Command is preferred when using Google Docs.
    Necessary Command content may be reused within the active Conversation.

13. **Command readiness.** Required Commands and dependencies must be usable for their assigned actions. An Agent must report missing definitions or inaccessible dependencies. It must not claim incomplete actions succeeded. Detailed execution mechanics remain with authorized implementation.

14. **Shared Execution foundation.** Execution Identities must apply shared Global Requirements.
    Assigned Instructions and applicable Commands must reflect each Identity's Responsibility and work type.
    Apply the common Role Lifecycle under Section 5.2.

15. **Shared Commands.** Identities with the same Role and Responsibility must share applicable Commands.
    Separate scoped Identities retain distinct scopes and own work records.
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
    For the user's own knowledge, Agents listen first under Section 1.1.5.
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

## 6. Meeting Lifecycle

### 6.1 Initialization and preparation

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
   Apply the user-supplied Context rule in Section 3.2.5.

5. **Opening.** Open the Meeting only after the user confirms its Agenda. Establish its Working Record and optional index. Verify those resources.

   Preserve:

   - Assigned Identity and Scope.
   - Actual Opening Time.
   - The confirmed Agenda.
   - Authoritative source references.

6. **Future Topic transfer.** Remove selected existing Future Topics only after their new Meeting Record is successfully established. Preserve unselected entries.

### 6.2 Discussion and outcomes

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
   The Working Record's persistence and QA boundary follows Section 9.1.

5. **Actions.** Identified Actions remain pending until their authorized execution phase unless the user explicitly authorizes earlier execution. Execute only actions within the Meeting Identity's own Responsibility and Scope. Prepare other Agents' work for handoff.

### 6.3 Closing and handoff

1. **Closing dispositions.** At CLOSE MEETING, present the following for disposition:

   - Unfinished Agenda items.
   - Deferred topics.
   - Out-of-scope matters.

   Carry-forward is the default proposal. Discard a candidate only through the user's explicit decision.

2. **Final Minutes.** Compile self-contained Final Minutes under Section 6.5 after completing the approved actions in Section 6.4.
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
   2. Consolidate qualifying Knowledge Base content under Section 3.3.
   3. Perform full-lifecycle Experience Capture.
   4. Send the authorized Handoff last.

   Each recipient applies its own Role Lifecycle, Scope selection and approval gates.
   Use Manual Handoff under Section 8.2.6 when Messaging is unavailable.

### 6.4 Post-Meeting Actions

1. **Own operating resources.** Meeting Identities maintain their own Context and current Working Records within governing rules.
   They may maintain applicable shared Knowledge Bases within their Responsibility and Scope.
   Identity Context maintenance follows Section 3.2.
   Knowledge Base maintenance follows Section 3.3.

2. **Other Deliverables.** Before editing other Deliverables or files, the Meeting Identity must obtain approval for the relevant Scope.
   Authority depends on Responsibility and approval, regardless of amendment size or file type.
   The Meeting Identity owns its approved Post-Meeting Actions and resulting Deliverables.

3. **Closing transition.** CLOSE MEETING initiates Closing and normal approved Post-Meeting Action execution.
   Finish every approved, Meeting-Agent-owned Post-Meeting Action before compiling Final Minutes.
   Preserve each action's actual outcome in the Working Record.
   Other Identities' work remains a separate authorized Handoff.
   Post-closure Knowledge Base consolidation follows Section 3.3.8.
   Apply the finalized record requirements in Section 6.3.3.

4. **Immediate execution.** Before Closing, execute an identified action only when the user expressly authorizes immediate execution.

   Discussion or confirmation of a required action alone does not authorize immediate execution.

### 6.5 Meeting artifacts

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

   Preserve accepted outcomes under Section 6.2 rather than a conversation transcript.
   Persistence follows Section 6.2.4.

4. **Final Minutes.** Final Minutes must have five Chapters:

   1. Meeting Information & Agenda.
   2. Confirmed Findings & Decisions.
   3. Actions & Outcomes.
   4. Open Matters & Dispositions.
   5. Sources & Quality Verification.

   Findings and Decisions share one substantive Chapter.
   Preserve their respective meaning under Section 6.2.3.
   Final Minutes must satisfy Global Writing Requirements and full Content, Writing and Formatting verification under Section 9.

5. **Minutes organization.** The Meeting Agent determines the internal subject grouping, heading hierarchy, order and presentation.
   Organize Final Minutes by related subject matter without requiring Agenda chronology.
   Related outcomes from different Agenda items may be consolidated.
   Preserve the full adopted substance.

## 7. Execution Parent Lifecycle

### 7.1 Stages and intake

1. **Shared forward flow.** The Execution Parent must use this sequence:

   1. NEW JOB / Information Intake.
   2. Scope Confirmation and Job Record.
   3. Proposal / Execution Plan.
   4. Execution Approval.
   5. Execution, with authoring, review, saving and registration of accepted Deliverables.
   6. Completion, with verification and Job finalisation.
   7. Context maintenance, Experience Capture and final communication under Section 7.3.

   Each step preserves its assigned owner and approval boundaries.

2. **Two approvals.** Obtain explicit confirmation of the selected Job Scope. Obtain separate PROCEED EXECUTION approval for the latest saved Execution Plan.

   Scope confirmation permits the following without another approval:

   - Record establishment.
   - Applicable Context maintenance.
   - Experience search.
   - Proposal preparation.

3. **Intake identity and sources.** Resolve identity during Initialization. Receive enabled Agent Messages. At NEW JOB, separately READ MESSAGES.

   Before interpreting a candidate's substantive Scope, read:

   - Relevant Identity Context.
   - Relevant scoped Knowledge Bases.
   - Work Requests.
   - The candidate's authoritative Closed Minutes.

4. **Previous checkpoint.** Consult the immediately preceding Job's last processed request or source checkpoint for the same exact Identity.
   Use the applicable indexed Scope when locating that record. Compare identifiers only within the same sequence. Preserve valid pending or excluded work.

5. **Future Execution work.** Automatically retain every valid Work Request not wholly incorporated into a confirmed Job.
   Keep pending work in the Execution Identity's Future Topics Chapter.
   Preserve each originating Identity and relevant source relationship.
   Remove unincorporated work only through explicit user direction.

6. **Pending entry content.** Each entry must contain:

   - Its Work Request identifier.
   - A specific Agent-authored Description.
   - Exact sources.
   - Relevant prerequisites.

   Derive the Description from the request and its Minutes. Keep it sufficient for continuation without duplicating the Minutes.

7. **Dependencies.** Verify dependencies against:

   - Completion Notices for the correct predecessor Agent or Job.
   - Requirements.
   - Sources.

   Classify each dependency using one of these states:

   - Completed.
   - Pending.
   - Unverified.

   Present unmet or unverified dependencies before Scope selection. The user may authorize earlier progress within actual technical and authority limits. Preserve the dependency's true state.

8. **Consolidated Job.** A Job may contain multiple confirmed Scopes from different originating Work Requests and Identities.
   Consolidate selected eligible Work Requests into the confirmed Job.
   The Job may contain multiple Deliverables.

   Reconcile:

   - Dependencies.
   - Overlap.
   - Supersession.
   - Conflict.

   Each Scope retains its originating Closed Minutes, source material and dependencies.
   Every Deliverable must retain its originating Identity, Work Request and source references.
   Present eligible Scope and useful combinations for the user's selection.
   Assign substantive execution under Section 7.4.

9. **Scope transition.** After Scope confirmation, establish and verify the Working Document and applicable Job index. Remove only incorporated portions from the retained future work after successful establishment. Retain partial and unselected remainders.

10. **Working Document.** Use “Working Document” as an environment-neutral term. Its physical form may differ by execution environment. A Job may use a fresh Conversation Context while preserving the durable Execution Identity Context.
    Apply the authoritative result-return requirements in Section 11.

### 7.2 Proposal and execution

1. **Proposal preparation.** Prepare one comprehensive Execution Plan for the entire Job:

   1. Read current target resources.
   2. Analyse every included Scope and its dependencies.
   3. Prepare the complete Execution Plan.
   4. Save the Plan.
   5. Present the saved Plan for approval.

   Every included Scope must be adequately planned before Job-level approval.
   The responsible author determines substantive organization and permitted implementation methods.
   Apply the Parent and Sub-agent responsibilities in Section 7.4.

2. **Plan content.** For each confirmed Scope, the saved Plan must identify:

   - Affected files or resources.
   - Planned impacts and their reasons.
   - Expected Deliverables and Outcomes.
   - Dependencies.
   - Sub-agent assignments and number.
   - Model choice.
   - PROFIT + A definitions.
   - QA criteria.
   - Completion conditions.

   Include ordered execution steps covering the entire Job.
   Preserve the authorship boundary in Section 7.4.3.

3. **Plan approval.** PROCEED EXECUTION approves the complete current saved Execution Plan once for the entire Job.
   Ordinary refinements may remain within approved requirements.
   Material Scope changes require a new Scope decision.
   Material changes to approved implementation require renewed Plan approval.

4. **Execution.** Check the approved Plan and required current resources. Perform only authorized work.

   Preserve:

   - Unrelated content.
   - Applicable Governance.
   - Child responsibility boundaries.

5. **Results.** Preserve the following in the Job Record:

   - Actual changes.
   - Outcomes.
   - Deliverable types.
   - Authoritative locations.
   - Necessary evidence.

   Maintain corresponding Job index references when Database services are enabled.
   Mandatory persistence checkpoints follow Section 7.5.7.

6. **Deliverable registration.** Register each Deliverable as soon as it is accepted and saved.
   When Database indexing is enabled, create or update its Document index with exact source and originating Job links.
   Verify existing indexes to avoid duplication.
   Required synchronization and verified Google Locators follow Section 11.
   The Database index may be created before the Identity Context Deliverable Index is updated.
   Update the Context Index immediately or consolidate it at Job close.

7. **Decision gaps.** A missing substantive decision must return to the Meeting process. Suspend the affected action until authoritative Closed Minutes resolve it. Preserve completed in-scope work. Deliverable organization and permitted implementation methods remain execution judgments.

### 7.3 Completion and communication

1. **Completion sequence.** Complete these actions in order:

   1. Verify actual saved Deliverables and their required registration.
   2. Verify the complete final Job Record and applicable indexes.
   3. Finalize the Job Record with the Completion Report, QA evidence and actual Job Done Time.
   4. Freeze the completed Job Record.
   5. Finalize and verify the existing Job index when enabled.
   6. Update Identity Context, including any remaining Deliverable Index updates.
   7. Optionally maintain relevant verified Knowledge Base content within approved authority.
   8. Perform full-lifecycle Experience Capture in the Experience Forum.
   9. Send relevant Completion Notices last.

   Apply System Rules and Database Atomic Actions to actual persistence and indexing.
   Knowledge Base maintenance remains discretionary for independently discovered knowledge under Section 3.3.7.

2. **Proof of Job.** A completed Working Document must preserve:

   - Approved Scope.
   - The source chain.
   - The Plan.
   - Approvals.
   - Actual changes.
   - Evidence.
   - Completion results.

   Where required, preserve actual times for:

   - Approval.
   - Execution.
   - Completion.

   Freeze the verified completed record as concise Proof of Job.

3. **Distinct outcomes.** Work across multiple Scopes or originating Identities must preserve each Deliverable's actual outcome and verification status.

4. **Completion authority.** Each executing Agent must perform its own internal QA under Section 9. Self-verification does not establish an independent Central QA assignment. Delegated execution also requires the Parent's independent acceptance under Section 7.4.

5. **After-Job recipients.** After verified formal Job closure, send a relevant Completion Notice to each originating Identity.
   Determine notices through each Deliverable's original Scope and Identity.
   Review every incorporated Work Request and its authoritative sources.
   Notify other directly related registered Identities when their current Responsibilities intersect the completed outcome.

   Resolve exact identities and relevance.
   Avoid unrelated or duplicate notices.
   Use Manual Handoff under Section 8.2 when Agent Messaging is unavailable.

### 7.4 Execution Parent and Sub-agents

1. **Substantive authorship.** When genuine Sub-agents are available, assign each Deliverable to a distinct genuine Sub-agent.
   Check actual creation and supervision capabilities.
   When the environment cannot create genuine Sub-agents:

   1. The Execution Parent authors the Deliverable.
   2. It performs a separate complete review pass.
   3. It labels the work as not delegated in the Job Record.

   Report actual capability limits accurately.
   A simulated Child must never be represented as genuine delegation.

2. **Parent control.** The Parent coordinates:

   - Job Scope.
   - Impact assessment.
   - The Execution List.
   - The managerial Proposal.

   It owns:

   - Approval gates.
   - Actual source collection.
   - Delegation.
   - Job supervision.

   Its final control responsibilities are:

   - Independent review.
   - Feedback.
   - Formal acceptance.
   - Final save/publication authorization.
   - Job closure.

   The Parent exclusively owns and writes the append-oriented Job Record.
   Sub-agents return candidates and evidence without modifying that Record.

3. **Execution List.** The Parent's Execution List identifies expected impact. Identify applicable targets from:

   - Files.
   - Documents.
   - Folders.

   It must not prescribe the Child's internal:

   - Chapters.
   - Sections.
   - Content plan.
   - Deliverable structure.

   An expressly prescribed structure in authoritative Minutes remains binding.

4. **Sources and authorship.** The Parent supplies complete applicable:

   - Scoped subject knowledge.
   - Instruction-bearing Closed Minutes.
   - Constraints.
   - Supporting sources.

   The Child independently determines:

   - Substantive revisions.
   - Wording.
   - Organization.
   - Permitted implementation methods.

5. **Child submission.** The Child must:

   1. Author the substantive Deliverable.
   2. Perform its own QA.
   3. Return the complete candidate.

6. **Independent review.** The Parent independently reviews the entire candidate at every submission and revision.

   Compare it with:

   - Complete sources.
   - Requirements.
   - Global Writing Requirements.
   - Applicable artifact quality rules.

7. **Feedback and retries.** A FAIL requires specific feedback. Allow at most five Child retries after the initial submission. After five unsuccessful retries, report the unpassed outcome for the user's decision. The Parent must not assume the Child's substantive authorship.

8. **Acceptance gate.** Only a fully accepted candidate may proceed to:

   - Authoritative saving.
   - Publication.
   - Indexing.
   - Completed Job status.

   Temporary review copies are not accepted Deliverables.

9. **Delegation arrangement.** Follow model decisions from authoritative Minutes where specified.
   Otherwise offer models available in the actual execution environment for user selection.
   Past model choices and delivery methods may inform nonbinding advisory Proposals.
   Reasoning level and technical arrangements follow applicable user decisions and available capabilities.

   The five-retry rule applies to genuine delegated execution.

### 7.5 Job Record

1. **Required Chapters.** The append-oriented Job Record must have five Chapters:

   1. Job Information.
   2. Confirmed Scope & Sources.
   3. Execution Plan & Approval.
   4. Execution & QA Log.
   5. Completion & Handoff.

   Parent writing authority follows Section 7.4.2.

2. **Job Information.** Chapter 1 must centralize essential Job Metadata and actual times for:

   - Scope Confirmation.
   - Plan Approval.
   - Execution Start.
   - Completion.

   This Chapter must not repeat Responsibility or the Record's own Locator.

3. **Confirmed Scope & Sources.** Chapter 2 must record each confirmed Scope and its exact:

   - Work Requests.
   - Closed Minutes.
   - Sources.
   - Dependencies.

4. **Execution Plan & Approval.** Chapter 3 must preserve the comprehensive Plan and its approval.
   Per-Scope Plan content follows Section 7.2.2.

5. **Execution & QA Log.** Chapter 4 must contain the chronological execution and QA account in one Chapter.
   The Parent determines when to append interim:

   - Observations.
   - Submissions.
   - Reviews.
   - Retries.
   - Progress.

   Each accepted Deliverable must retain relevant execution and QA evidence.
   Full review and retry requirements follow Section 7.4.

6. **Completion & Handoff.** Chapter 5 must report completed work through each Deliverable, its corresponding Scope and actual Activity.
   The Parent determines remaining evidence, detail and organization.
   The account must remain accurate, complete and verifiable without a rigid field-by-field template.

7. **Mandatory persistence.** Save and verify these checkpoints:

   1. Scope confirmation.
   2. The complete Execution Plan.
   3. Plan approval.
   4. Accepted Deliverable results and relevant evidence.
   5. Final Job Completion.

## 8. Records, Messaging, and Experiences

### 8.1 Records and interface authority

1. **Durable records.** Agents should preserve appropriate durable evidence for:

   - Substantive Meetings.
   - Scope establishment.
   - Agent assignments.
   - Identity changes.

   This does not require a separate document for every small action.

2. **Index meaning.** Database records must index authoritative content rather than duplicate document bodies.

   Record categories distinguish:

   - Meetings.
   - Jobs.
   - Actual Documents.

   Agent Role and exact Agent Identity identify responsibility separately from resource type.

3. **Index verification.** Indexed sources must use exact authoritative locators and verified returned identifiers.

   Previous Job lookup must distinguish:

   - Applicable indexed Scope.
   - Job category.
   - Exact Agent Identity.

   Preserve historical sources and unresolved identity uncertainty.

4. **Database Contracts.** The Execution Identity assigned Database Engineering must maintain authoritative interface definitions for approved database services. Applicable operating Contracts must expose only needed operations and shared semantics. Commands own when and why interfaces are used.

   Contracts own:

   - Inputs.
   - Behavior.
   - Outputs.
   - Relevant integrity or security constraints.

5. **Engineering verification.** Approved database changes must preserve applicable:

   - Integrity.
   - Security.
   - Transaction safety.
   - Interface compatibility.

   Verify:

   - Actual behavior.
   - Affected data.
   - Contract consistency.

   Add complexity only when a real requirement supports it.

### 8.2 Messaging

1. **Identity and routing.** Enabled Agent Messaging must use exact registered sender and recipient identities.

   Resolve recipients from the central System Context registry using:

   - Registered Identity.
   - Responsibility.
   - Work type.
   - Scope reference.
   - Relevance.

   Hold ambiguous recipients pending.

2. **Work Requests.** A Work Request must identify:

   - Its authorized origin.
   - Bounded Scope.
   - The exact recipient.
   - Authoritative sources.

   The recipient must apply its own Scope selection and execution approvals.

3. **Completion Notices.** A Completion Notice must report:

   - Verified completed work.
   - The outcome.
   - The authoritative record.
   - Deliverable references.
   - Recipient relevance.

   Send it only after the full assigned Protocol completes. It must not instruct the recipient or create new execution authority.

4. **Message handling.** Distinguish newly received Messages from historical search results. Preserve sources and essential meaning. Present suggested follow-up as a proposal. Message search must preserve read state according to the applicable Contract.

5. **Delivery evidence.** The Messaging System maintains delivery evidence.
   Verify stored Message identifiers and timestamps.
   Reuse the same request key for an uncertain identical retry when supported.
   Stored delivery does not prove recipient reading.
   Exact routing identities do not authenticate individual Agents.
   A frozen Job Record need not be reopened merely to store later Message IDs.

6. **Manual Handoff.** Without Database Messaging, the sending Agent supplies copy-ready Handoff text.
   Include relevant authority, source references and actual outcomes.
   The user pastes it into the receiving Agent's Conversation.
   The receiving Agent records it in its own Future Topics.
   Preserve normal responsibility, Scope and approval boundaries.

### 8.3 Experience learning

1. **Advisory status.** Experiences must remain advisory.

   Assess the following against current authoritative requirements:

   - Evidence.
   - Applicability.
   - Freshness.
   - Scope.
   - Limitations.

   They cannot override:

   - Governing decisions.
   - Instructions.
   - Approvals.
   - Assigned Scope.

2. **Execution checkpoints.** After confirmed Job Scope and successful record establishment, SEARCH EXPERIENCES once before Proposal preparation. After verified Job finalisation, CAPTURE EXPERIENCE once for the entire Job before After-Job communication.

   Search during work only for one or more of:

   - Genuine difficulties.
   - Corrections.
   - Relevant quality problems.

3. **Meeting checkpoints.** Meeting operations retain applicable Experience searches at Protocol Start and near completion.
   Perform one full-lifecycle Capture after post-closure Knowledge Base consolidation and before the final Handoff.
   The closing sequence follows Section 6.3.7.

4. **Capture outcomes.** Compare actual reusable learning with governing sources and existing Posts.

   Verify:

   - Evidence.
   - Novelty.
   - Limitations.

   Then publish, replace, react or conclude that no action is needed.
   Experience Capture publishes only to the Experience Forum for both Meetings and Jobs.
   No Experience entry is required in frozen Job Records or Minutes.
   Do not publish merely because a Protocol ended.

5. **Experience quality.** Authored Topic names and Post content must follow Strict Mode writing requirements.

   Preserve:

   - Circumstances.
   - User intent.
   - The actual result.
   - Evidence.
   - Limitations.
   - Future applicability.

   Reactions must reflect actual application. Counts do not establish instruction authority.

## 9. Deliverable quality and independent QA

1. **Actual artifacts.** Every Agent must verify the latest saved version of each Deliverable it creates or modifies.
   Verification of a Working Document does not replace verification of separate Deliverables.

   Final Minutes and other Deliverables require full Content, Writing and Formatting verification.
   Meeting Working Records require accurate, verified persistence under Section 6.2.4.
   They require neither mandatory Global Writing Requirements document QA nor a Quality Checklist.

2. **Three dimensions.** Verify these dimensions separately:

   - Content Quality.
   - Writing Compliance.
   - Formatting Compliance.

   Content includes:

   - Completeness.
   - Correctness.
   - Approved Scope.
   - Source fidelity.

   Writing follows active Global Writing Requirements and the correct Writing Mode. Formatting follows the artifact format and applicable Operating Guide. Apply output-specific checks required by the assigned role and deliverable.

3. **Evidence.** For every artifact subject to full QA, record actual PASS or FAIL for each affected dimension.
   Record permitted corrections and successful verification of the latest saved version.
   Read the complete final artifact after substantive changes before claiming compliance.

   After all modifications, independently inspect the complete Requirements artifact across the three quality dimensions in Section 9.2.

4. **Formatting checkpoints.** Verify Formatting after creating and saving Job Records and Final Minutes.
   Verify final Formatting again at Protocol completion.
   Routine edits need not each trigger a full Formatting check.
   Meeting Working Records follow Section 9.1.

5. **Easy to Read.** Formatting must provide:

   - Readable hierarchy.
   - Natural information flow.
   - Visual balance.
   - Quick navigation.

   It must help intended readers:

   - Follow the artifact.
   - Understand it.
   - Scan it.

   Apply the rules for whichever artifact format applies:

   - Google Docs.
   - Markdown.
   - Other formats.

6. **Operating Guides.** Where needed, a Document Operating Guide must own its document's:

   - Purpose.
   - Names.
   - Metadata.
   - Sections.
   - Formatting.
   - Local QA criteria.

   Lifecycle actions and cross-resource execution belong in Commands. Apply structural refinements prospectively while preserving historical records and approved formats.

7. **Writing meaning.** Written outputs must preserve meaningful:

   - Modality.
   - Confidence.
   - Conditions.
   - Qualifications.

   Give each part one semantic purpose. Keep authoritative meaning in its owning location.

   Remove:

   - Duplication.
   - Unsupported claims.
   - Obsolete wording.
   - Unnecessary negative echo.

8. **Writing clarity.** Use clear, direct wording. Maintain established terminology consistently. Prefer active voice and one independent instruction per sentence. Keep paragraphs focused and no longer than six sentences. Use structured lists for three or more comparable items.

9. **Strict Mode.** Apply Strict Mode to:

   - The entire Requirements file, including retained content, additions, consolidation and future revisions.
   - Authoritative governing and operational artifacts.
   - Sub-agent Prompts.
   - Plugin Development Prompts.
   - Agent Messages.
   - Experience content.

   Limit instructional sentences to 20 words and descriptions to 25 words unless precision requires otherwise. Avoid semicolons and phrasal verbs. Keep controlled terms grammatically consistent.

10. **Language.** English is the default for:

    - Operating instructions.
    - Controlled terminology.
    - Database search values.

    Authored content may use another language or mixed languages according to purpose and audience. Preserve original authoritative sources when translations exist. Apply active user communication settings in Conversation.

11. **Independent QA Scope.** The Identity assigned Central QA must inspect every approved item at the authorized depth.

    Possible dimensions include:

    - Structure.
    - Operating Guide compliance.
    - Requirement fidelity.
    - Decision-to-Deliverable Fidelity.
    - Context authority.

    Writing Compliance is compulsory for substantively inspected or authored documents subject to full QA under Section 9.1.

12. **Fidelity inspection.** Compare full substantive meaning, including:

    - Intent.
    - Requirements.
    - Constraints.
    - Qualifications.
    - Approved revisions.

    Identify:

    - Omissions.
    - Weakening.
    - Excessive editing.
    - Unauthorized additions.
    - Changed requirements.

    Trace the earliest verified divergence and its downstream effect. Source citations alone do not establish fidelity.

13. **QA reporting.** Each inspected item needs:

    - Exact source and target references.
    - Criteria.
    - Evidence.
    - Findings.
    - A result using one of these statuses:
      - PASS.
      - FAIL.
      - Unable to Verify.

    Fidelity findings must identify a useful correction starting point and final impact. Report inadequate evidence without presuming compliance.

14. **Independent QA limits.** Complete every approved audit item without cached PASS reuse or automatic skipping. QA reports identify deficiencies but do not authorize correction. A completed audit may contain failed or unverifiable findings.

## 10. Reusable development Workflows

### 10.1 Purpose, progression, and foundation

1. **Reusable Workflow.** The Plugin must include the existing Book Development Workflow as a shared Task/Deliverable resource.

   Approved Scope selects its application. Governing working arrangements may define applicable:

   - Outputs.
   - Locations.
   - Assigned Agents.

2. **Author intent.** Develop the user's fragmented or conversational input while preserving core thinking and intended meaning. Contribute new ideas only when explicitly requested.

3. **Stages and owners.** Guide one active Book through these stages:

   1. The Book Meeting Agent develops Book Foundation and Outline with the user.
   2. It saves confirmed outcomes to the Book Knowledge Base.
   3. The shared Execution Agent drafts the manuscript with complete QA.
   4. The user reviews the draft in a Meeting.
   5. Apply revisions under Section 5.22 and continue until the rough manuscript is complete.
   6. Complete Content Edit and Copy Edit under Section 10.3.
      Apply the revision ownership rule in Section 5.22 to both edits.

   Earlier stages may be revisited when new information materially changes the Book.
   Change the active Book only through explicit user direction.
   Default drafting and permitted Chapter customization follow Section 5.21.

4. **Purpose.** Before manuscript development, clarify WHY the user wants to write the book and WHY NOW it matters.

   Use this purpose when any of these conditions applies:

   - Choices compete.
   - Confidence falls.
   - Direction is lost.

5. **Book Idea.** Establish one main Book Idea and singular focus.

   If the Book Idea is unclear, explore:

   - Expertise.
   - Paid work.
   - Deep interests.
   - Recurring requests for advice.
   - Repeated questions or conversations.

   When ideas compete, consider:

   - Fastest completion with existing material.
   - Likelihood of finishing.
   - Motivation.
   - Satisfaction.

6. **Ideal Reader and 4Ps.** Clarify four reader and positioning decisions:

   1. **Person.** Identify the specific reader for one or more of these purposes:
      - Helping that reader.
      - Entertaining that reader.
      - Reaching that reader.
   2. **Pain.** Identify one or more things the reader already recognizes:
      - A problem.
      - A need.
      - A tension.
      - A desire.
   3. **Promise.** Identify one or more intended results the reader should receive:
      - An outcome.
      - A benefit.
      - An experience.
      - Value.
   4. **Price.** Identify the intended price or pricing position for the book's genre and format.

   Use Person as the primary writing reference.

   Align the following with that reader:

   - Voice.
   - Examples.
   - Explanations.
   - Stories.
   - Detail.

   Fiction and children's books may address the user or readers seeking their intended genre or experience.

### 10.2 Architecture and Chapter development

1. **Living architecture.** Maintain one living Book Architecture supporting discovery through a Mind Map and structure through an Outline. Exhaust relevant material before perfecting structure.

   Capture:

   - Ideas.
   - Stories.
   - Experiences.
   - Examples.
   - Evidence.
   - Lessons.
   - Repeated explanations.
   - Reference-triggered ideas.

2. **Progressive organization.** Early material may have any of these qualities:

   - Messy.
   - Repetitive.
   - Incomplete.
   - Unordered.

   Organize it progressively.

   Sequence the following for natural reader progression:

   - Parts.
   - Chapters.
   - Supporting points.

   Do not delay drafting to perfect the first architecture.

3. **Nonfiction structure.** Identify major themes or Parts, usually three to seven broad Sections where useful. Organize Chapters and supporting points beneath them. Give an idea its own Chapter only when its meaning justifies one.

4. **Fiction structure.** Where applicable, establish this story progression:

   1. **Set-Up.** Establish:
      - The hero.
      - Motivation.
      - Setting.
      - Genre.
      - World rules.
      - Major conflicts.
      - Important tropes.
   2. **Inciting Incident.** This event changes the hero's path and cannot simply be ignored.
   3. **First Slap.** This stage escalates the stakes severely.
   4. **Second Slap with Hope.** This stage further escalates events while revealing possible progress or victory.
   5. **Climax.** Connect it to the Inciting Incident. Resolve the central conflict appropriately.

5. **Optional Chapter loop.** When the Identity customizes a large Book for Chapter-by-Chapter drafting, use:

   1. Content Extraction.
   2. Chapter Structure.
   3. Confirmation.
   4. Chapter Draft.

   Use focused questions to elicit the user's:

   - Thinking.
   - Experiences.
   - Stories.
   - Examples.
   - Reasoning.
   - Intended effect.

   Do not replace missing core ideas without explicit permission to contribute.

6. **Structure confirmation.** Within the customized Chapter loop, identify before drafting:

   - Chapter purpose.
   - The key message.
   - Supporting points.
   - Stories or examples.
   - Sequence.

   Confirm meaning and structure with the user before drafting from them.

7. **Chapter Draft.** Draft confirmed material point by point for the Ideal Reader. Develop author voice from the user's communication and confirmed direction. Accept spoken or conversational input. Organize that material into coherent prose. When using the customized Chapter loop, repeat it until the rough manuscript is complete.

### 10.3 Manuscript completion and review

1. **Rough drafting.** Complete the book's meaning before polishing language. Capture improvements for later rather than repeatedly editing unfinished Chapters. Maintain a practical completion plan using Chapter or time checkpoints where useful.

2. **Drafting boundaries.** Unless explicitly included, protect rough drafting from:

   - Title work.
   - Cover work.
   - Marketing.
   - Launch work.
   - Publishing work.

   Preserve blocked gaps or placeholders and continue where possible.

3. **Momentum.** When momentum falls, revisit:

   - WHY.
   - WHY NOW.
   - The active stage.
   - The next concrete step.

   Review or adjust completion goals under user direction. Restore a sustainable writing commitment. Offer accountability support when useful. An imperfect complete rough draft satisfies the completion priority better than isolated polished Chapters.

4. **Author Review.** After rough completion, perform at least one complete review from the Ideal Reader's perspective. Prefer verbal review when practical because listening may reveal problems missed during silent reading.

   Identify:

   - Errors.
   - Gaps.
   - Insufficient stories or supporting material.
   - Unclear meaning.
   - Departures from author voice or intent.

   Treat discomfort with the first complete draft as part of the creative process.

   When direction is lost, revisit:

   - Purpose.
   - Ideal Reader.
   - Promise.

   Progress when sufficiently ready for Content Edit.

5. **Content Edit.** Resolve:

   - Content gaps.
   - Tangents.
   - Duplication.
   - Flow.
   - Transitions.
   - Supporting material.
   - Sequence.
   - Unclear meaning.

   Assess fulfillment of the Promise for the Ideal Reader.

   When justified, choose one or more appropriate actions for the material:

   - Move it.
   - Merge it.
   - Expand it.
   - Remove it.
   - Restructure it.

   Before sentence polishing, resolve:

   - Meaning.
   - Content.
   - Structure.

6. **Copy Edit.** Begin when content and structure are sufficiently settled.

   Improve:

   - Spelling.
   - Grammar.
   - Punctuation.
   - Redundancy.
   - Wording.
   - Clarity.
   - Flow.
   - Consistency.
   - Readability.

   Preserve confirmed:

   - Meaning.
   - Voice.
   - Promise.

7. **Finished Manuscript.** Require content-level and copy-level review.

   Treat the book as finished when it is:

   - Clear.
   - Coherent.
   - Readable.
   - Consistent.
   - Fit for the Ideal Reader.

   Apply a practical completion boundary rather than endless polishing.

8. **Book State.** Keep Book progress in the owning Identity Context under Section 5.21:

   - The active stage.
   - The current Part or Chapter.
   - Open content gaps.
   - The next step.

   Keep confirmed Book decisions in the Book Knowledge Base under Section 5.19.

### 10.4 Book Deliverables and Language Editions

1. **Standard Book Workflow.** The Book ownership and language-cycle requirements in Section 10 belong in the standard Book Development Workflow.
   Book Meeting Minutes and Job Records follow the standard records in Sections 6 and 7.
   The manuscript is one Deliverable containing its Chapters.

2. **Base Edition.** One Book cycle produces one finished manuscript in the Base Edition language.
   Complete and publish the Base Edition before beginning an additional-language cycle.

3. **Language Editions.** Each additional language is a separate cycle.
   Redraft each Language Edition from the final Base Edition manuscript and Book Knowledge Base.
   A Language Edition is a redraft, not a translation.

### 10.5 Business Document Development Workflow

1. **Brief and structure.** The Meeting Agent works with the user to:

   1. Agree the document brief.
   2. Gather sources.
   3. Confirm the structure.

   The user makes final decisions under Section 5.22.

2. **Full draft and QA.** The shared Execution Agent writes one full draft.
   Every draft includes its own complete QA under Section 9.
   The user reviews each draft in a Meeting.
   Apply the revision ownership rule in Section 5.22.

3. **Numbered revisions.** Each revision produces a new numbered draft based on:

   - The previous draft.
   - Relevant Closed Minutes.
   - Relevant Knowledge Bases.

4. **Stable version.** When the user approves a draft, the Meeting Agent records it as the Stable version in the Minutes.
   The Stable version is the baseline for later drafts.
   It may be sent to a client or another reader under applicable authorization.

5. **Reference knowledge.** Each document draws on one or more Knowledge Bases appropriate to its subject.
   Examples include:

   - Brand.
   - Company profile.
   - Product.

   Select the content the document needs and write it appropriately.
   Do not copy whole Knowledge Base contents into the document.
   The Meeting Agent maintains the relevant Knowledge Bases and Minutes so redrafts preserve confirmed meaning.

6. **Document types.** Main types include:

   - Proposals.
   - Plans.
   - Policies.
   - Resolutions.
   - Letters.
   - Emails.
   - Other business communication or proposal documents.

## 11. Environments, result return, and governed changes

1. **Execution environments.** The architecture must support authorized work through:

   - ChatGPT.
   - Local environments.
   - Future independent machines.

   Execution surfaces may use their own Working Documents and assets. Plugin packaging alone does not establish native operation on every host.

2. **Connectors.** Every participating environment must have suitable Google Drive / Docs access. Host-specific integrations and System Rules select the actual connector.
   Local integration selections remain environment-specific.
   Local Agents may use Agent Messaging when available. The AI must assess required setup and permissions according to its actual environment.

3. **Governance continuity.** Local and remote work must preserve:

   - Authoritative Google decisions.
   - Approved Scope.
   - The Plan.
   - Agent boundaries.
   - Required approvals.

   Local files do not establish independent governance authority.

4. **Result return.** Return the following to the owning Google-authoritative workflow:

   - Required Job or Execution Record details.
   - Actual status.
   - Results.
   - Necessary evidence.
   - Deliverable references.

   At required completion checkpoints, synchronize applicable local outputs to designated Google locations.
   Local System Rules determine which outputs synchronize.
   Verify required updates before claiming completion.
   Eligible Database Record indexing follows required synchronization and uses accessible, verified Google Locators.
   Full workspace copies and every intermediate asset are not automatically required.

5. **Access limitations.** Report unavailable authoritative access or uncompleted required updates accurately. Discuss permitted setup or assistance with the user. Detailed operational access-restoration behavior remains subject to later practical design.

6. **Governed implementation.** System and Scope changes must follow:

   - Their authorized owner.
   - Source authority.
   - Scope confirmation.
   - The saved Proposal.
   - Execution approval.

   Synchronization must preserve:

   - Current governing decisions.
   - Approved customization.
   - Active work.
   - Records.
   - Valid pending requests.

   Verify affected resources and outcomes independently.

## 12. Baseline acceptance and deferred development

1. **Foundation acceptance.** The initial foundation must provide:

   - A usable Repository entry.
   - A concise README.
   - Consolidated Requirements.
   - Durable source traceability.

   Verify:

   - Confirmed meaning.
   - Current coverage.
   - Authority.
   - Readability.
   - Approved Scope.
   - Actual saved outputs.

   Apply artifact-specific checks for:

   - Content.
   - Writing.
   - Formatting.

2. **Subsequent Plugin work.** Actual Plugin development must follow the requirements baseline under a separately authorized development Job. A working Plugin and full Documentation are not mandatory initial foundation outputs.

3. **Remaining resource mechanics.** Additional resource mechanics and unusual ownership exceptions require later authorized design.
   Preserve the adopted ownership, consolidation and record requirements in Sections 3, 5, 6 and 7.

4. **Deferred Workflows.** These remain future reusable Workflows:

   - Website Development.
   - Governance.
   - Code Development.

   Their detailed stages remain undecided.
   Preserve the standard Book and Business Document outcomes in Section 10.
   Refine permitted methods through practical experience without changing confirmed flow requirements.

5. **Remaining implementation design.** The following require later authorized design:

   - Exact packaging.
   - Update methods.
   - Remaining resource schemas and Registry details.
   - Source-refresh mechanics.
   - Further environment arrangements.
   - Google and Local System Rules Templates.
   - Precise Workflow invocation.
   - Google and cross-environment Locator schemas.
   - Optional Database configuration and credential details.

   Preserve current confirmed outcomes without inventing missing substantive decisions.

6. **Migration boundary.** Existing Projects Migration remains a separate later workstream after Framework development.

   Its future direction includes:

   - Preservation of historical records.
   - Review of current information.
   - Recreation of Projects in the new structure.
   - Import of reviewed context and Archive.

   Historical material does not automatically override current governance. Database redesign and any transition require independent authorization and verified preservation.

