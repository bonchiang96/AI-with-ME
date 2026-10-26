# AI with ME - Operating Framework

AI with ME - Operating Framework is a portable, instruction-led Framework for AI work. It combines:

- Reusable Plugin instructions.
- Authoritative Google governance resources.
- Optional Database services.

The design preserves user decisions within assigned responsibilities. It maintains durable continuity across Conversations and execution environments.

## 1. Development status and navigation

This repository is the authoritative development and distribution source for the Plugin and reusable operating resources.

| Location | Purpose | Status |
| --- | --- | --- |
| [Requirements V1](requirements/requirements.md) | Consolidated requirements for Framework development. | Available |
| `plugin/` | The installable Plugin with shared operating resources and installation guidance. | Planned |
| `documentation/` | Detailed operating guidance and reference material. | Planned |

The current deliverables are the repository foundation and Requirements V1. The Requirements define the adopted design. Runtime implementation follows separately approved work.

## 2. Operating concept

1. **Identity and continuity.** The user selects an operational Identity from central Google System Context. Each Identity has a registered Role. Its Responsibility and Scope define its assignment. Its central Google Identity Context holds current operating information and references for continuing work. Agents discover relevant progress and sources before asking the user to reconstruct prior work.

2. **Roles and Workflows.** Meeting Agent and Execution Agent are the two principal Roles. Each Identity uses its Role's shared Lifecycle. A Workflow guides a particular Task or Deliverable. Standard Workflows reside in the Plugin, while user-created Workflows may reside in scoped Knowledge Bases. Without a suitable Workflow, Agents use their available capabilities under the assigned Role Lifecycle and existing approval requirements.

3. **Meetings and decisions.** Meeting Agents organize discussion and confirmed decisions. Each Meeting has an append-oriented Working Record and separate, self-contained Final Minutes. Accepted outcomes are saved and verified at each Agenda boundary. Final Minutes follow completed approved Meeting-owned actions and receive full Content, Writing and Formatting verification. The Working Record requires verified persistence, without mandatory Global Writing Requirements document QA or a Quality Checklist.

4. **Governed execution.** An Execution Parent consolidates selected work into a Job, preserving each Scope's sources. The user confirms Scope and separately approves one complete saved Execution Plan with PROCEED EXECUTION. Each Deliverable has a distinct genuine Sub-agent for substantive execution. The Parent owns the Job Record and independently reviews every complete submission and revision. Only accepted Deliverables proceed to publication after Content, Writing and Formatting PASS.

   Relevant Completion Notices follow verified completion of the full Role Protocol, including formal Job closure.

5. **Scoped knowledge.** Knowledge Bases hold current subject knowledge for their defined Scopes and may serve multiple Identities. Agents may maintain independently discovered, sufficiently verified knowledge whenever useful. Qualifying user-confirmed knowledge must be consolidated from verified Closed Minutes after Meeting closure. Historical evidence remains in its original Records and Minutes.

   Execution Agents use relevant Knowledge Bases for current subject knowledge. They use specific authoritative Closed Minutes for work instructions.

6. **Shared instructions.** The intended installed Plugin supplies reusable resources for normal operation without routine GitHub reads. Current governance and operating references come from their Google authority.

The [Requirements](requirements/requirements.md) provide the complete operating specification.

## 3. Environments and dependencies

The design supports authorized work through:

- ChatGPT.
- Local environments.
- Future independent machines.

Each environment needs suitable Google Drive / Docs access and granted permissions. Host-specific integrations determine the actual connector.

1. **Required: Google Drive / Docs.** Google System Context centrally registers Identities and Knowledge Bases. Local environments use the assigned central Identity and its authoritative Context. Google System Rules govern Google-side document persistence.

2. **Optional: Database.** Database services may support:

   - Indexes.
   - Search.
   - Agent Messaging.
   - Handoff.

   System Context holds suitable connection references, while applicable System Rules govern enablement. Without Database services, Agents provide copy-ready Manual Handoff when appropriate. If Supabase is selected, research current official setup guidance when needed.

Local System Rules govern actual local working resources and determine which outputs synchronize to Google. Local Bootstrap establishes missing Local System Rules and required working paths only.

Applicable System Rules override conflicting Plugin instructions for these environment operations:

- Storage.
- Synchronization.
- Database Atomic Actions.

Applicable outputs synchronize to designated Google locations at required completion checkpoints. Verify required synchronization before eligible Database indexing, using accessible, verified Google locators. Local Agents need not reread Google for every ordinary file operation.

## 4. Installation, System entry and updates

### 4.1 Installation and updates

The intended distribution lets users create, manually install and manually update their own Private Plugin from this repository.

When the Plugin becomes available:

1. Provide this repository's URL to an AI.
2. The AI reads this README and locates the Plugin and installation guidance in `plugin/`.
3. The AI assesses dependencies and assists installation using available tools and granted permissions.

The AI must explain unavailable capabilities or permissions. It must discuss the next authorized step. GitHub supplies source for intentional updates. Installation and update guidance will be discoverable here as those deliverables become available.

### 4.2 System entry

The central Google Drive System Root is named “AI with me”. Use existing accessible resources for normal operation.

When the initial Root or required System resources are confirmed missing, a provisional System Meeting Identity begins a Bootstrap Meeting. It explains the proposed resources and responsibilities. The user confirms the arrangement before separately authorized Execution establishes and registers the resources. Local environments use this central Root.

## 5. License

This repository uses the [MIT License](LICENSE).
