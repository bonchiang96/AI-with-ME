# Foundation

Return to the [Requirements Overview](README.md).

## 1. Repository, distribution, and installation

1. **Source authority.** One GitHub Repository must be the authoritative development and distribution source for the Plugin and reusable operating resources. Maintain their common instructions in that source.

2. **README.** The root README must explain the Framework for its readers in plain words.
   Use [Global Writing Requirements](global-writing-requirements.md) Standard Mode.

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

## 2. Governance resources and dependencies

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
   Bootstrap follows [System, Identity and Entry Section 1.2](02-system-identity-and-entry.md#1-identity-selection-and-governed-setup).

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
   Rule priority follows [Section 2.8](#2-governance-resources-and-dependencies).

5. **Resource purposes and destinations.** Governing configuration must define known deliverables and meaningful destinations.
   For each maintained resource, identify the necessary:

   - Purpose.
   - Expected outcome.
   - Location.
   - Responsible Identity.

   Identity Context must reference its own applicable record destinations under [Section 3.3](#3-identity-context).
   Storage follows [Section 2.4](#2-governance-resources-and-dependencies).

6. **Workflow customization.** Governed working arrangements may customize a Workflow's:

   - Stage outcomes.
   - Deliverables.
   - Target Locations.
   - Assigned maintenance responsibilities.

   These arrangements may evolve through confirmed decisions and practical work.
   Preserve Role Lifecycle authority under [System, Identity and Entry Section 2.2](02-system-identity-and-entry.md#2-agent-responsibilities-and-commands).

7. **Context discovery.** An Identity must open its own Identity Context to discover relevant:

   - Records.
   - Collaboration partners.
   - Deliverables.
   - Working references.

   System Context supplies the registered Identity Context Locator.

8. **Contextual priority.** Applicable System Rules override conflicting Plugin instructions for the environment operations in [Section 2.4](#2-governance-resources-and-dependencies).

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

12. **Database-free operation.** Without Database services, Agents must omit unavailable Database-dependent operations. Apply the manual handoff requirements in [Records, Messaging and Experiences](05-records-messaging-and-experiences.md). Identity discovery and essential governance must remain possible through Google resources.

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

    Add fields only when they serve a genuine directory purpose. Keep each directory compact. Identity Context current references follow [Section 3](#3-identity-context).

## 3. Identity Context

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
   Register accepted and saved Deliverables under [Execution Lifecycle Section 2.6](04-execution-lifecycle.md#2-proposal-and-execution).
   The creating Execution Identity may update its Context Index immediately or consolidate updates at Job close.
   A Meeting Identity may refresh its relevant Index after receiving a Completion Notice at a later Meeting.

5. **User-originated decisions.** User-originated decisions require appropriate authoritative support.
   User-confirmed Meeting matters enter authoritative Identity Context only after verified Closed Meeting Minutes.
   Preserve the relevant source reference.

6. **Working Group.** Working Group may retain real collaboration selected by relevant participants.
   It may include useful Identity pairings and collaboration patterns.
   The Agent determines useful maintenance timing through judgment.
   User-originated decisions follow [Section 3.5](#3-identity-context).

7. **Selected current references.** Identity Context may preserve useful:

   - Workflow references.
   - Useful Workflow usage.
   - The current Workflow stage.
   - Related Minutes.
   - Meaningful verified accomplishments.

8. **Organization.** Each Identity controls content organization within the six required Chapters.
   Keep each Chapter's meaning within its purpose.

## 4. Scoped Knowledge Base

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
   - User-created Workflows permitted under [System, Identity and Entry Section 2.19](02-system-identity-and-entry.md#2-agent-responsibilities-and-commands).

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
   2. Identity operating information belongs in Identity Context under [Section 3](#3-identity-context).
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
   4. Apply [Global Writing Requirements](global-writing-requirements.md) Standard Mode.
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
