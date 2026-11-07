---
name: knowledge-base
description: Discovers, creates, consolidates and maintains AI with ME scoped Knowledge Bases and Deliverable Guidelines, and runs Experience search, Learning Candidates and Experience capture. Covers semantic routing of Closed Minutes, the routing test for Experiences, the Knowledge Base folder index and the Identity Context Knowledge Bases Chapter. Use when a Lifecycle needs subject knowledge, post-closure consolidation, a Deliverable Guideline or Experience learning.
compatibility: Requires the Google Drive and Google Docs connectors through the host. The Plugin does not ship the connectors.
---

# Knowledge Base

## 1. Purpose

A Knowledge Base stores knowledge for a defined Scope.
There are two kinds:

1. **Scoped Knowledge Bases** store external subject information for a defined Scope.
   Examples are a company, a Brand, a Book or a specialist domain.
   One Scope may hold several scoped Knowledge Bases.
2. **The general Knowledge Base** stores Experience only.
   Each Experience must improve the System across projects, not serve one project only.

Several Identities may use or maintain the same Knowledge Base. No Knowledge Base belongs to an Identity.

## 2. Location

1. Every Knowledge Base resides in the Knowledge Base folder under the System Root.
2. The folder holds a [00 Index](../../templates/knowledge-base-index.md) with one line per Knowledge Base.
   Its three columns are Name, Location and Description.
3. It holds the [general Knowledge Base](../../templates/general-knowledge-base.md) to which every Identity contributes Experience.
4. It holds every scoped Knowledge Base.

## 3. Format

A Knowledge Base has a free format. Its headings must be numbered. Use Heading styles, not bold text.
Create a new Knowledge Base from the [general Knowledge Base](../../templates/general-knowledge-base.md) layout.
The Operating Guide always keeps the six template items: Purpose, Names, Metadata, Sections, Formatting and Local QA criteria.
Put Scope and authority statements inside Purpose. Never replace the Operating Guide with another structure.

## 4. Discovery

Read each level only when needed:

1. The Knowledge Bases Chapter of Identity Context.
2. The Knowledge Base folder index.
3. The contents list of each Knowledge Base.

Read Knowledge Bases on demand. A relevant topic, a circumstance or a user request decides when.
Reuse content already loaded in the Conversation. Read it again only when it is not enough or the user asks.

Execution uses relevant scoped Knowledge Bases for current subject knowledge.
Execution uses the Deliverable Guideline for current Deliverable guidance.
Execution uses the specific Closed Minutes for work instructions.

## 5. Content

A scoped Knowledge Base includes only currently valid content within its Scope:

- Confirmed external subject knowledge.
- User-created Workflows.

The general Knowledge Base includes only currently valid Experience under Section 11.

Preserve adopted future directions as future directions.

When the source records Rationale or Design Intent, keep it with the knowledge it explains.
Keep only the reasons for the current truth. Do not record why older content was replaced.
Exclude exploratory ideas, unresolved choices, superseded content, future Jobs and Deliverable progress.

These never belong in a Knowledge Base:

- Deliverable copy or drafts, such as website text. These belong in the Deliverable.
- Guidance on how to produce a Deliverable. This belongs in its Deliverable Guideline.
- Task assignments, such as who is responsible for an action.
- Job or Meeting status, and statements that a Meeting will decide something.
- Agent instructions and Lifecycle rules. These belong in the Plugin or System Rules.
- History and correction wording, such as "previously", "corrected", "legacy", "此前", "最新纠正" or "旧".
- Lists of Minutes links used as a source chapter.

Routing check: when content tells the reader what to do for a Deliverable, it goes to the Deliverable Guideline.

## 6. Maintenance triggers

1. **Discretionary.** An Agent may maintain independently discovered, sufficiently verified subject knowledge whenever useful.
2. **Mandatory.** After a Meeting closes, consolidate qualifying user-confirmed Topic or Scope knowledge from the verified Closed Minutes.
3. **Missing scoped Knowledge Base.** When qualifying knowledge has no applicable scoped Knowledge Base, create one under Section 9.

Execution completion alone does not trigger scoped Knowledge Base maintenance.

## 7. Post-closure consolidation

Flow: verified Closed Minutes → classify each outcome → route each part → consolidate → save and verify.

1. Review the entire Closed Minutes.
2. Classify each confirmed outcome by its actual meaning. One Decision may hold several parts.
3. Route each part to its owner:
   1. External subject knowledge goes to an applicable scoped Knowledge Base.
   2. Guidance for a Deliverable goes to its Deliverable Guideline under Section 12.
   3. Future Topics and High-Priority Items go to Identity Context.
   4. Governance goes to its authoritative resources.
   5. Job-specific instructions remain in the Closed Minutes and Job authority.
4. Mentioning a working Scope does not make an instruction subject knowledge.
5. Save and verify the result independently.
6. Do not reopen or modify the Minutes.

This consolidation is routine post-closure maintenance, not a Post-Meeting Action.
Experience is handled separately under Section 11.

## 8. Consolidation method

1. Read the complete current Knowledge Base.
2. For Closed-Minutes-based work, also read the new verified Closed Minutes.
3. Consolidate throughout the complete resource. Do not append. Keep every heading numbered.
4. Retain all valid knowledge.
5. Integrate newly confirmed subject matter.
6. Replace only genuinely superseded content. Replace its Rationale and Design Intent with those of the new truth.
7. Apply Standard Mode under the [global-writing-rules](../global-writing-rules/SKILL.md) Skill.
8. Include useful paragraph-level source references where helpful.
   Place each reference inside its paragraph. Never continue a block with new content after its source line.
9. Scan for duplicates. Each fact appears in one place. Other places use a short cross-reference.
10. After the last change, read the complete saved Knowledge Base and verify it.
    Check the Operating Guide against the template, the heading styles and the contents list.
11. Verify its line in the 00 Index.

Ordinary updates do not require the full Historical Minutes collection.

## 9. Index and Identity Context lines

1. When an Identity creates a Knowledge Base, it adds the index line with Name, Location and Description.
2. The Description tells an Agent or a person what the Knowledge Base covers.
   When the Knowledge Base's Topic changes, any Identity may update the Description.
   The Description changes only then.
3. Update the Identity Context Knowledge Bases Chapter at these points:
   - Identity setup.
   - Knowledge Base creation.
   - Use of a newly found source.
   - Discovery of a broken link.
4. Each Chapter entry has Name, Location and Relation. Relation is Uses or Contributes.

## 10. Experience search

1. Search through the discovery levels in Section 4.
2. In a Job, search once after Scope confirmation and record establishment, before Proposal preparation.
3. During a Job, search only for genuine difficulties, corrections or relevant quality problems.
4. In a Meeting, search at step 4 of NEW MEETING, before the Agenda, and at step 3 of CLOSE MEETING.
5. Experiences remain advisory.
6. Assess evidence, applicability, freshness, Scope and limitations against current requirements.
7. Experiences cannot override governing decisions, instructions, approvals or assigned Scope.

## 11. Experience

### 11.1 Kinds of Experience

1. **Failure Experience.** It arises when the user asks for a change or correction, or states that the Agent got something wrong.
2. **Success Experience.** It arises when the user states that something was good.
   Identify the pattern behind the success, such as the planning, the thinking or the method.
   State the pattern so it can apply widely.

### 11.2 Learning Candidates

1. Record each failure or success as a Learning Candidate when it happens.
2. Record it in the Meeting Record of the Meeting or the Job Record of the Job.
3. Each Learning Candidate states what happened, the user's words or intent, and the lesson or pattern.
4. A Learning Candidate is a working note. It is routed only at capture.

### 11.3 Routing test

Route each Experience by whom it helps:

1. **Helps this Identity work better.** It goes to the Important Learning Chapter of this Identity's Identity Context.
2. **Helps the user and other Identities work better.** It goes to the general Knowledge Base.
3. **External subject knowledge** found during the work goes to a scoped Knowledge Base under Section 7.

One Experience goes to one target. The more general target applies when it helps other Identities.

A general Knowledge Base Experience states a project-neutral lesson.
Keep the project name in its Source reference.
Keep a short example only when it helps the reader understand, in one sentence.
Merge Experiences that share one lesson.

### 11.4 Capture

1. In a Meeting, capture once after scoped Knowledge Base and Deliverable Guideline consolidation, before the Identity Context update.
2. In a Job, capture once after verified Job finalization, before the Identity Context update.
3. Review every Learning Candidate and the whole Meeting or Job for further Experience.
4. Compare each Experience with governing sources and existing Knowledge Base content.
5. Verify evidence, novelty and limitations.
6. Apply the routing test in Section 11.3.
7. Consolidate each general Knowledge Base contribution under Section 8.
8. Pass each Identity-level Experience to the Identity Context update.
9. Preserve circumstances, user intent, the actual result, evidence, limitations and future applicability.
10. Apply each Experience directly to its target. No record stores the routing.

Frozen Job Records and Minutes need no Experience entry.

## 12. Deliverable Guideline

### 12.1 Purpose

A Deliverable Guideline holds the complete current guidance for one Deliverable.
It tells the Execution Agent what to produce and why each guidance point exists.
Every Deliverable has a Guideline, whatever its Workflow, including work done without a Workflow.

### 12.2 Rules

1. Every rule in this Skill for Knowledge Bases applies to the Guideline. It has no separate rule set.
2. It holds current truth only. Exclude historical and superseded content.
3. Keep Rationale and Design Intent with each guidance point.
4. Use the Knowledge Base format in Section 3.
5. Its content depends on the Deliverable. No Workflow fixes a Guideline content template.

### 12.3 Owner and timing

1. The Meeting Agent that governs the Deliverable creates and maintains the Guideline.
2. Create it at the Meeting that decides the Deliverable.
3. Consolidate it after every review Meeting, from the verified Closed Minutes.
4. Guideline consolidation runs beside scoped Knowledge Base consolidation under Section 7.

### 12.4 Arrangement and location

The arrangement is guidance, not a hard rule.
The Meeting Agent proposes the arrangement for each Deliverable. The user confirms it.

1. **Default.** One Deliverable has one Guideline.
   In a Google Docs Deliverable, Tab 1 is the Guideline and the following Tabs hold the drafts.
   In another storage place, such as local, the Guideline is a file beside the Deliverable.
2. **Many Guidelines.** A Deliverable may need many Guidelines, such as a Book drafted Chapter by Chapter.
   One Guideline document may then hold them all. The Deliverable is a separate file.
3. The Guideline resides in the Deliverable's agreed storage place.
4. The 01 Index registers the Deliverable only. The Guideline needs no separate index entry.

### 12.5 Use in execution

1. The Handoff to the Execution Agent names the Guideline link and the latest Closed Minutes.
   In Google, the link is the Guideline Tab link.
2. The Execution Agent produces the Deliverable from the Guideline and the relevant Knowledge Bases.
