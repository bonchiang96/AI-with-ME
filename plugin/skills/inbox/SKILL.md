---
name: inbox
description: Reads, processes and sends AI with ME inbox messages. Covers Work Requests and Completion Notices between registered Identities through each Identity's 02 Inbox Google Docs file. Use when an Agent Lifecycle reads its inbox at NEW MEETING or NEW JOB, or sends a Handoff or Completion Notice.
compatibility: Requires Google Drive and Google Docs access through a host connector.
---

# Inbox

## 1. Purpose

Agents exchange Work Requests and Completion Notices through inbox files.
Each Identity has its own 02 Inbox. No Identity merges another Identity's inbox.
The file follows the [Inbox template](../../templates/inbox.md).

Flow: sender writes one row → sender verifies the row → receiver reads at start → receiver routes the outcome → receiver deletes the row.

## 2. Routing

1. Use exact registered sender and recipient Identities.
2. Resolve recipients from the System Context registry by Identity, Responsibility, work type, Scope reference and relevance.
3. Hold ambiguous recipients pending.
4. Exact routing Identities do not authenticate individual Agents.

## 3. Message types

1. A Work Request identifies its authorized origin, bounded Scope, exact recipient and authoritative sources.
2. The recipient applies its own Scope selection and execution approvals.
3. A Completion Notice reports verified completed work, the outcome, the authoritative record, Deliverable references and recipient relevance.
4. Send a Completion Notice only after the full assigned Protocol completes.
5. A Completion Notice does not instruct the recipient or create execution authority.

## 4. Sending

1. Add one row to the recipient's 02 Inbox.
2. Fill Sent, From, Type, Ref and Message.
3. Ref is the key of a closed record in the sender's 01 Index.
4. Write the Message in Strict Mode under the [Global Writing Rules](../../rules/global-writing-rules.md).
5. Verify the saved row.
6. A saved row does not prove that the recipient has read it.

## 5. Reading and processing

Read the inbox at the start order step of the [meeting-agent](../meeting-agent/SKILL.md) or [execution-agent](../execution-agent/SKILL.md) Lifecycle.

1. Open the record that each row references.
2. Route the outcome to every relevant place:
   - Route pending Work Requests to Future Topics under the execution-agent Lifecycle.
   - Route Deliverables to the 01 Index under the meeting-agent Lifecycle.
3. Delete the processed row.
4. Preserve sources and essential meaning.
5. Present suggested follow-up as a proposal.
6. Preserve normal responsibility, Scope and approval boundaries.

An unwritable inbox is a failure-handling matter. Use judgment within authorized Scope and report necessary assistance.
