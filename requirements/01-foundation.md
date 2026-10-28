# Foundation

Return to the [Requirements Overview](README.md).

## 1. Repository, distribution, and installation

1. **Source authority.** One GitHub Repository must be the authoritative development and distribution source for the Plugin and reusable operating resources. Maintain their common instructions in that source.

2. **README.** The root README must explain the Framework for its readers in plain words.
   Use [Global Writing Rules](global-writing-rules.md) Standard Mode.

   Include:

   - What the Framework is and why it exists.
   - One simple flow picture.
   - Required and optional dependencies.
   - A short getting-started section.
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
   - Standard templates and Operating Guides under [Section 6](#6-templates-and-operating-guides).

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

   The package is the plugin folder with two manifests.
   An update reinstalls the Plugin from a chosen commit.

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

## 2. Governance resources and dependencies

1. **Google authority.** Google Drive / Docs is the authority for governance, records, indexes and inbox messages.
   Hybrid local working and Deliverable storage follow [Environments and Acceptance Section 2](07-environments-and-acceptance.md#2-hybrid-local-working-and-deliverable-storage).

   This authority applies across:

   - ChatGPT.
   - Local environments.
   - Future independent AI execution.

2. **System Root.** The central Google Drive System Root must be named “AI with me”.
   It must provide access to:

   - Central System Context.
   - Applicable System Rules.
   - Identity folders under [Section 5.1](#5-identity-folder-index-and-inbox).
   - The Knowledge Base folder under [Section 4.9](#4-scoped-knowledge-base).
   - Resources for registered working Scopes.

   Environment System Rules govern their actual storage structure.
   Local environments must use this central Root rather than create another System Root.
   Bootstrap follows [System, Identity and Entry Section 1.2](02-system-identity-and-entry.md#1-identity-selection-and-governed-setup).

3. **System Context.** Google System Context must provide central authority for Identity registration.
   Its Registry must list one Locator per Identity: its identity folder under [Section 5.1](#5-identity-folder-index-and-inbox).
   System Context must also reference the Knowledge Base folder and its index under [Section 4.9](#4-scoped-knowledge-base).
   Maintain one authoritative registration per Identity, including its assigned Responsibility and Scope.
   Local environments must use the assigned central Identity without creating a separate Local Identity Registry.

   Preserve current System configuration.
   Routine progress belongs in its owning records or current Identity references.

4. **System Rules.** System Rules must express user-defined shared operating conventions.
   Google System Rules must govern Google-side:

   - Document creation.
   - Locations and storage structure.
   - Resource maintenance.

   Google System Rules start with these starter rules:

   1. Create documents as Google Docs with native tables.
   2. Name each Tab with the pattern date — Topic — key, such as 2026-10-27 — Plugin Build — J-0256.
   3. Write each date and time as YYYY-MM-DD HH:MM in 24-hour time with the time-zone abbreviation, such as 2026-10-27 19:45 MYT.

   Local System Rules contents follow [Environments and Acceptance Section 2.2](07-environments-and-acceptance.md#2-hybrid-local-working-and-deliverable-storage).

   Apply the rules for the actual execution environment.
   A further inbox Type is a customization added through System Rules under [Section 5.5](#5-identity-folder-index-and-inbox).
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
   Preserve Role Lifecycle authority under [System, Identity and Entry Section 2.2](02-system-identity-and-entry.md#2-agent-responsibilities-stage-words-and-workflows).

7. **Context discovery.** An Identity must open its own Identity Context and index to discover relevant:

   - Records.
   - Collaboration partners.
   - Deliverables.
   - Working references.

   System Context supplies the registered identity folder Locator.

8. **Contextual priority.** System Rules take priority over the Plugin.

   Interpret other governing overlap using:

   - Context.
   - Purpose.
   - Source authority.
   - Known intent.
   - The situation.

   An exhaustive override matrix or mechanical conflict algorithm is not required.

9. **Source loading.** Agents should reuse static instructions available in the effective Conversation Context unless their applicability changes.
   They must read dynamic context and working data when current information is needed.
   Load applicable Plugin Skills selectively at the relevant Lifecycle stage.
   Local Agents need not reread Google for each ordinary file operation.

10. **Meaningful resources.** Every maintained resource should serve an identified purpose. Resource creation must follow authorized Responsibility, Scope and actual operating needs.

11. **Indexes.** Each Identity keeps its index as a Google Docs file under [Section 5.2](#5-identity-folder-index-and-inbox).

12. **Handoff.** Agents exchange Work Requests and Completion Notices through inbox files.
    Inbox use follows [Records, Messaging and Experiences Section 2](05-records-messaging-and-experiences.md#2-messaging).
    Identity discovery and essential governance must remain possible through Google resources.

13. **Integration expression.** Integration requirements must identify:

    - The authoritative resource.
    - The necessary action.
    - The expected output.
    - Applicable constraints.

    Connector invocation methods belong to the executing AI.

14. **Identity directory.** Each Identity entry in System Context has these fields:

    - Agent Key.
    - Role.
    - Responsibility and Scope, in one line or a few sentences.
    - Location of the identity folder.

    Add fields only when they serve a genuine directory purpose. Keep each directory compact. Identity Context current references follow [Section 3](#3-identity-context).
    Index files, the Knowledge Base folder index and Identity Context lists follow their own templates.

15. **Google Locator.** A Google Locator is the Google Docs link of a file.
    For a Tab, the Google Locator is the Tab link.

## 3. Identity Context

1. **Starting context.** Every Identity must maintain one consolidated central Google Identity Context as its starting context for work.
   It contains current working information, future work and operating references.
   It is not described as memory.
   Complete historical evidence belongs in its original Records and Minutes.
   Local environments use this authoritative Context without creating a duplicate Local Context.
   It is the 00 Identity Context file in the identity folder under [Section 5.1](#5-identity-folder-index-and-inbox).

2. **Required Chapters.** Identity Context must contain these six Chapters:

   1. Operating Guide.
   2. Future Topics.
   3. Working Group.
   4. Important Learning.
   5. Important Things or High-Priority Items.
   6. Knowledge Bases.

   The Operating Guide follows [Section 6](#6-templates-and-operating-guides).
   Working Group contains peer Identities and Handoff relationships.
   Knowledge Bases follows [Section 3.9](#3-identity-context).
   Metadata follows [Section 3.10](#3-identity-context).

3. **Own record locations.** The identity folder holds the Identity's own Minutes, Working Records and Job Records under [Section 5.1](#5-identity-folder-index-and-inbox).
   Identity Context must reference applicable Target Locations for additional Identity-owned records or resources.

   Distinguish sources for reading from authorized record-writing destinations.

4. **Verified operating information.** An Identity may update its independently derived information whenever useful within its Responsibility and Scope.
   Deliverable registration follows [Section 5.4](#5-identity-folder-index-and-inbox).

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

9. **Knowledge Bases Chapter.** The Knowledge Bases Chapter lists each Knowledge Base the Identity uses or contributes to.
   Each entry has these fields:

   - Name.
   - Location.
   - Relation, with the value Uses or Contributes.

   Update the list at these points:

   1. Identity setup.
   2. Knowledge Base creation.
   3. Use of a newly found source.
   4. Discovery of a broken link.

10. **Metadata.** Identity Context metadata holds:

    - The Agent Key.
    - The Role.
    - The identity folder location.

    Responsibility and Scope stay only in System Context under [Section 2.14](#2-governance-resources-and-dependencies).

## 4. Scoped Knowledge Base

1. **Knowledge resources.** A Knowledge Base must store external subject information for a defined Scope.
   Examples include:

   - A company.
   - A Brand.
   - A specialist domain.

   One Scope may contain multiple Knowledge Bases.
   Multiple Identities may use or maintain the same Knowledge Base.
   No Knowledge Base belongs to an Identity.
   Any Identity may add the Knowledge Base folder index line when it creates a Knowledge Base.
   Any Identity may update the line's Description when the Knowledge Base's Topic changes.
   The Description changes only then.

2. **Current content.** Include only currently valid content within the Knowledge Base's Scope:

   - Confirmed external subject knowledge.
   - User-created Workflows permitted under [System, Identity and Entry Section 2.16](02-system-identity-and-entry.md#2-agent-responsibilities-stage-words-and-workflows).

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
   Consolidate every contribution, including Experience, into the existing content rather than appending it.
   Ordinary updates do not require rereading the full Historical Minutes collection.

   During consolidation:

   1. Retain all valid knowledge.
   2. Integrate newly confirmed subject matter.
   3. Replace only genuinely superseded content.
   4. Apply [Global Writing Rules](global-writing-rules.md) Standard Mode.
   5. Useful paragraph-level source references may be included.

6. **Execution sources.** Execution must use relevant scoped Knowledge Bases for current subject knowledge. It must also use the specific authoritative Closed Minutes for work instructions. Execution completion alone does not trigger Knowledge Base maintenance.

7. **Maintenance triggers.** Apply these two distinct triggers within the Knowledge Base's Scope:

   1. An Agent may maintain independently discovered, sufficiently verified subject knowledge whenever useful.
      This maintenance is discretionary.
   2. Qualifying user-confirmed Topic or Scope knowledge must be consolidated from verified Closed Minutes after the Meeting closes.
      This maintenance is mandatory when qualifying content exists.

   Experience contribution follows [Records, Messaging and Experiences Section 3](05-records-messaging-and-experiences.md#3-experience-learning).

8. **Post-closure maintenance.** Closed-Minutes-based consolidation is routine post-closure maintenance rather than a pre-Minutes Post-Meeting Action.
   Save and verify its result independently.
   It must not reopen or modify immutable Minutes.

9. **Knowledge Base folder.** Every Knowledge Base resides in the Knowledge Base folder under the System Root.
   The folder holds:

   - A 00 Index with one line per Knowledge Base.
     Its three columns are Name, Location and Description.
     The index tells an Agent or a person which Knowledge Bases exist and what each covers.
   - A general Knowledge Base to which every Identity contributes.
   - Every other Knowledge Base.

10. **Knowledge Base discovery.** Discovery uses three levels. Read each level only when needed:

    1. The Knowledge Bases Chapter of Identity Context under [Section 3.9](#3-identity-context).
    2. The Knowledge Base folder index.
    3. The contents list of each Knowledge Base.

    Agents read Knowledge Bases on demand. A relevant topic, a circumstance or a user request decides when.
    Agents reuse content already loaded in the Conversation. They read it again only when it is not enough or the user asks.

11. **Knowledge Base format.** A Knowledge Base has a free format.
    Its headings must be numbered.

## 5. Identity folder, index and inbox

1. **Identity folder.** Each Identity has one identity folder. The folder holds these numbered files:

   1. 00 Identity Context under [Section 3](#3-identity-context).
   2. 01 Index under [Section 5.2](#5-identity-folder-index-and-inbox).
   3. 02 Inbox under [Section 5.5](#5-identity-folder-index-and-inbox).

   A Meeting Agent folder also holds 03 Working Records and 04 Minutes.
   An Execution Agent folder also holds 03 Job Records.
   Index and inbox files are Google Docs with native tables.
   Identity setup creates every file with its Operating Guide under [System, Identity and Entry Section 1.11](02-system-identity-and-entry.md#1-identity-selection-and-governed-setup).

2. **Index file.** Each Identity has its own index file, separate from Identity Context.
   The index lists only closed records: Final Minutes and closed Job Records.
   Chapter order depends on the Role:

   - A Meeting Agent index holds Deliverables first, then Meetings.
   - An Execution Agent index holds Jobs only.

3. **Index keys and columns.** Each key uses a letter and a number, such as M-0003:

   - D for Deliverable.
   - M for Meeting.
   - J for Job.

   Keys carry no Identity key.
   Each Chapter uses these template columns:

   - Deliverables: Key, Title, Type, Location, Condition, From.
   - Meetings: Key, Date, Topic, Final Minutes location, one-line Outcome.
   - Jobs: Key, Date, Scope, Job Record location, From, one-line Outcome.

   A From cell names the sender Identity and its record key, linked to that record.
   In the Jobs Chapter, the From cell names the sending Meeting the same way.
   The index lists what exists. It is not a live tracker.
   Google version history shows when a row changed.
   Each Identity may amend its columns through Minutes.

4. **Deliverable rows.** A Deliverable row records a package or set rather than every file.
   A new version leaves the index unchanged.
   Condition values are Draft, Stable, Frozen and Archived.
   The originating Meeting Agent registers a Deliverable when it processes the Completion Notice.
   Register a Deliverable package when it first appears.
   Changes inside an indexed package need no index change.
   The Agent judges when an index or Identity Context update is needed.

5. **Inbox file.** Each inbox row has five columns:

   1. Sent.
   2. From, which names the sender Identity.
   3. Type.
   4. Ref, which is the key in the sender's index.
   5. Message.

   Inbox Types are Work Request and Completion Notice.
   A further Type is a customization added through System Rules.
   Inbox use follows [Records, Messaging and Experiences Section 2](05-records-messaging-and-experiences.md#2-messaging).

## 6. Templates and Operating Guides

1. **Operating Guide placement.** Every file has an Operating Guide. Place it as follows:

   - The first Chapter of System Context, System Rules, Identity Context, index and inbox files.
   - The first Tab of Working Record, Final Minutes and Job Record files.
   - A 00 Operating Guide file in the folder for any other file.

   Operating Guide content follows [Quality Section 1.6](06-quality.md#1-deliverable-quality-and-independent-qa).

2. **Standard templates.** The Plugin ships standard templates and Operating Guides.
   Agents adjust them with the user rather than inventing them.
   No template or created file may hold placeholder text.
