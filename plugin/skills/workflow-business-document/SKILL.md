---
name: workflow-business-document
description: The standard AI with ME Business Document Development Workflow. Covers proposals, plans, policies, resolutions, letters, emails and other business documents. Takes each document from brief and sources through numbered full drafts with QA and user review to a Stable version. Use when the user selects the Business Document Workflow for a Task.
compatibility: Requires the Google Drive and Google Docs connectors through the host. The Plugin does not ship the connectors.
---

# Business Document Development Workflow

## 1. Use

1. The user selects this Workflow when a Task starts. The Agent may propose it.
2. Main document types are proposals, plans, policies, resolutions, letters, emails and other business communication or proposal documents.
3. Each Identity runs its own steps under its Role Lifecycle.
4. Keep the current stage in the Identity Context of the Agent that owns the current step.
5. Transfer stage ownership only through a normal Handoff.

Flow: brief and structure → full draft with QA → user review in a Meeting → numbered revision → Stable version.

## 2. Brief and structure

The Meeting Agent works with the user to:

1. Agree the document brief.
2. Gather sources.
3. Confirm the structure.

The user makes final decisions. Leave space for user input. Advise when asked or when direction is unclear.

## 3. Full draft and QA

1. The shared Execution Agent writes one full draft.
2. Every draft includes its own complete QA under the [workflow-qa](../workflow-qa/SKILL.md) quality dimensions.
3. The user reviews each draft in a Meeting.
4. Apply the user review and revision rule in [meeting-agent](../meeting-agent/SKILL.md).

## 4. Numbered revisions

Each revision produces a new numbered draft based on:

- The previous draft.
- Relevant Closed Minutes.
- Relevant Knowledge Bases.

## 5. Stable version

1. When the user approves a draft, the Meeting Agent records it as the Stable version in the Minutes.
2. The Stable version is the baseline for later drafts.
3. Sending the Stable version to a client or another outside reader still needs applicable authorization.
   A Stable status alone does not authorize sending.

## 6. Reference knowledge

1. Each document draws on one or more Knowledge Bases appropriate to its subject, such as Brand, company profile or product.
2. Select the content the document needs and write it appropriately.
3. Do not copy whole Knowledge Base contents into the document.
4. The Meeting Agent maintains the relevant Knowledge Bases and Minutes so redrafts preserve confirmed meaning.
