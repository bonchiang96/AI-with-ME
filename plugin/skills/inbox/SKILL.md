---
name: inbox
description: Reads, processes and sends AI with ME inbox messages. Covers Work Requests, Completion Notices and Information between registered Identities through each Identity's 02 Inbox Google Docs file. Use when an Agent Lifecycle reads its inbox at NEW MEETING or NEW JOB, or sends a Handoff or Completion Notice.
compatibility: Requires the Google Drive and Google Docs connectors through the host. The Plugin does not ship the connectors.
---

# Inbox

## 1. Purpose

Agents exchange Work Requests, Completion Notices and Information through inbox files.
Each Identity has its own 02 Inbox. No Identity merges another Identity's inbox.
The file follows the [Inbox template](../../templates/inbox.md).

Flow, part 1: sender writes one row → sender verifies the row.
Flow, part 2: receiver reads at start → receiver routes the outcome → receiver deletes the row.

## 2. Routing

1. Use exact registered sender and recipient Identities.
2. Resolve recipients from the System Context registry by Identity, Responsibility, work type, Scope reference and relevance.
3. Hold ambiguous recipients pending.
4. Exact routing Identities do not authenticate individual Agents.

## 3. Message types

The inbox Types are Work Request, Completion Notice and Information.
A further Type is a customization added through System Rules.

1. A Work Request identifies its authorized origin, bounded Scope, exact recipient and authoritative sources.
2. The recipient applies its own Scope selection and execution approvals.
3. A Completion Notice reports verified completed work, the outcome, the authoritative record, Deliverable references and recipient relevance.
4. Send a Completion Notice only after the full assigned Protocol completes.
5. A Completion Notice does not instruct the recipient or create execution authority.
6. Information only informs the recipient. Use it for any matter the recipient should know.
   Examples: you used the recipient's work, or something the recipient owns may need a change.
7. Information does not request work or report a completed Job. It creates no execution authority.

## 4. Sending

1. Add one row to the recipient's 02 Inbox.
2. Fill Sent, From, Type, Ref and Message.
   Write Sent in the date and time format of the Google System Rules.
3. Ref is the key of a closed record in the sender's 01 Index.
   For Information without a related record, leave Ref empty and give the source link in the Message.
4. Write the Message in Strict Mode under the [Global Writing Rules](../global-writing-rules/SKILL.md).
   Reference the record. Never copy a document body into the Message.
   Send only after the record is in Google and its Deliverable is in the agreed place.
5. Verify the saved row.
6. A saved row does not prove that the recipient has read it.

## 5. Reading and processing

Read the inbox at the start order step of the [meeting-agent](../meeting-agent/SKILL.md) or [execution-agent](../execution-agent/SKILL.md) Lifecycle.

1. Open the record that each row references.
2. Route the outcome to every relevant place:
   - Route pending Work Requests to Future Topics under the execution-agent Lifecycle.
   - Route Deliverables to the 01 Index under the meeting-agent Lifecycle.
   - For Information, update your own context when relevant. Any resulting work follows your own Lifecycle.
3. Delete the processed row.
4. Preserve sources and essential meaning.
5. Present suggested follow-up as a proposal.
6. Preserve normal responsibility, Scope and approval boundaries.

An unwritable inbox is left to your judgment. Act within authorized Scope and report necessary assistance.
