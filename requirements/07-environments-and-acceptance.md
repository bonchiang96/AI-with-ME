# Environments and Acceptance

Return to the [Requirements Overview](README.md).

## 1. Environments, result return, and governed changes

1. **Execution environments.** The architecture must support authorized work through:

   - ChatGPT.
   - Local environments.
   - Future independent machines.

   Execution surfaces may use their own Working Documents and assets. Plugin packaging alone does not establish native operation on every host.

2. **Connectors.** Every participating environment must have suitable Google Drive / Docs access. Host-specific integrations and System Rules select the actual connector.
   Local integration selections remain environment-specific.
   Local Agents use the inbox under [Records, Messaging and Experiences Section 2](05-records-messaging-and-experiences.md#2-messaging). The AI must assess required setup and permissions according to its actual environment.

3. **Governance continuity.** Local and remote work must preserve:

   - Authoritative Google decisions.
   - Approved Scope.
   - The Plan.
   - Agent boundaries.
   - Required approvals.

   Local files do not establish independent governance authority.

4. **Result return.** Return the following to the owning Google-authoritative workflow:

   - Required Job Record details.
   - Actual status.
   - Results.
   - Necessary evidence.
   - Deliverable references.

   Local work returns to Google under [Section 2](#2-hybrid-local-working-and-deliverable-storage).
   Verify required updates before claiming completion.
   Record index rows use accessible, verified Google Locators.
   Deliverable index rows identify the agreed storage place under [Section 2.6](#2-hybrid-local-working-and-deliverable-storage).
   Full workspace copies and every intermediate asset are not automatically required.

5. **Access limitations.** Report unavailable authoritative access or uncompleted required updates accurately. Discuss permitted setup or assistance with the user.
   Access restoration is left to AI judgment under [Requirements Overview Section 2.4](README.md#2-binding-non-functional-requirements).

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

## 2. Hybrid local working and Deliverable storage

1. **Hybrid local working.** Agents may run Meetings, Jobs and development locally.
   Google Drive remains the authority.

2. **Local System Rules.** Local System Rules reside in the Local System Rules Chapter of Google System Rules.
   Local System Rules must govern:

   - The local folder and its arrangement.
   - Local file formats.
   - Naming.
   - Directories and working paths.
   - Local Record creation.
   - Local Deliverable creation.
   - When and how work returns to Google.

3. **Local folder arrangement.** The local root holds one folder per Identity, named by its Agent Key.
   Each Identity folder holds one folder per Meeting or Job.
   Each Meeting or Job folder is named like its Google Tab under [Foundation Section 2.4](01-foundation.md#2-governance-resources-and-dependencies).

4. **Google-only resources.** These resources always stay in Google:

   - System Context.
   - Identity Context.
   - The index.
   - The inbox.

5. **Record return.** Records return to Google at these points:

   1. The Working Record and Final Minutes return at Meeting close.
   2. The Job Record returns at Job completion.

6. **Deliverable storage.** A Deliverable is stored where it fits, such as Google Drive, GitHub or GitLab.
   The index Location identifies that place.
   The Meeting agrees each Deliverable's storage place with the user.
   The Meeting records that place in the Final Minutes.
   The Execution Plan lists it.

7. **Missing storage place.** When no storage place is recorded, the Execution Agent asks the user at Scope confirmation.

8. **Indexing and announcement.** Nothing is indexed or announced until both conditions are met:

   1. Its record is in Google.
   2. Its Deliverable is in the agreed place.

## 3. Baseline acceptance

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

2. **Plugin work.** Plugin development must follow the Requirements baseline under an authorized development Job.
