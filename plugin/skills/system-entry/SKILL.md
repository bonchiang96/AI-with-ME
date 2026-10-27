---
name: system-entry
description: Starts every AI with ME Conversation. Checks the Google Drive and Google Docs connectors and locates the "AI with me" System Root. Opens System Context, lets the user select a registered Identity and loads its Role Lifecycle and Identity Context. Runs Bootstrap when the System Root is confirmed absent. Use at the start of every Conversation or when the user asks to enter the AI with ME System.
compatibility: Requires Google Drive and Google Docs access through a host connector. The Plugin does not ship the connectors.
---

# System Entry

## 1. Purpose

This skill brings each Conversation from its start to a selected, loaded Identity.
The outcome is an Identity ready for NEW MEETING or NEW JOB.

Flow: connector check → locate System Root → open System Context → read System Rules → select Identity → load Role Lifecycle and Identity Context → ready.

## 2. Rules for every reply

1. Apply the [Global Communication Rules](../../rules/global-communication-rules.md).
2. Apply the [Global Writing Rules](../../rules/global-writing-rules.md).
3. Read these rule files from the Plugin, not from Google Drive.

## 3. Connector check

1. Check Google Drive and Google Docs access in the actual environment.
2. Google Drive / Docs is the only storage for governance, records, indexes and inbox messages.
3. When a connector, capability or permission is unavailable, explain the practical limitation to the user.
4. Discuss the next authorized step.
5. Perform or guide permitted setup within your capabilities.
6. Do not claim that an incomplete action succeeded.

## 4. Entry flow

1. Locate the central Google Drive folder named “AI with me”.
2. Open System Context in that folder.
3. Assess access to the applicable System Rules.
4. Read the user overrides in the applicable System Rules once.
5. Reuse existing accessible resources.
6. Present the active registered Identities from System Context.
7. The user selects one Identity.
8. Load the skill for that Identity's Role:
   - Meeting Agent: [meeting-agent](../meeting-agent/SKILL.md).
   - Execution Agent: [execution-agent](../execution-agent/SKILL.md).
9. Open the Identity's 00 Identity Context through its registered identity folder.
10. Load applicable System Rules and Plugin instructions for the assignment.
11. Discover current information before asking the user for it again.

The Identity is then ready for NEW MEETING or NEW JOB.

## 5. Identity resolution

1. Accept a directly supplied Identity Context Locator or a registered Identity resolved through System Context.
2. Both paths must reach the Identity Context through the identity folder.
3. Resolve the user's assignment against registered Scope information.
4. Resolve a missing or ambiguous Identity before scoped Messaging.
5. Do not default an unresolved scoped assignment to another Identity.
6. Inactive or archived Identities stay out of normal active choices.
7. An inactive or archived Identity may be reactivated when appropriate.

Detailed cross-environment Locator design is pending design.

## 6. Bootstrap

Bootstrap runs only when the System Root is confirmed absent.

1. Inaccessibility alone does not prove absence.
2. Resolve access or location uncertainty before creating another Root.
3. A default provisional Meeting Agent holds a Bootstrap Meeting under the [meeting-agent](../meeting-agent/SKILL.md) Lifecycle.
4. The provisional Identity needs no Registry entry.
5. Bootstrap records remain in the Conversation until the folder exists.

In the Meeting, explain the proposed:

- Root.
- System Context.
- System Rules.
- Knowledge Base folder.
- Responsibilities.
- Minimum Identities.
- Creation actions.

The user approves the System arrangement and its creation actions in that Meeting.
After CLOSE MEETING, the same Meeting Agent performs these Post-Meeting Actions:

1. Create the folder.
2. Create System Context and System Rules from the [System Context](../../templates/system-context.md) and [System Rules](../../templates/system-rules.md) templates.
3. Create the Knowledge Base folder with its [00 Index](../../templates/knowledge-base-index.md) and [general Knowledge Base](../../templates/general-knowledge-base.md).
4. Establish the two minimum Identities under the Identity setup in [meeting-agent](../meeting-agent/SKILL.md):
   - The General Meeting Agent, with Agent Key `general-meeting`.
   - The General Execution Agent, with Agent Key `general-execution`.
5. Save the Bootstrap Working Record and Final Minutes as the System's first records.
6. Join the normal entry flow at Identity selection.

Restore genuinely missing resources within existing approved authority and applicable System Rules.

## 7. Local environments

1. Local environments use the central System Root, System Context and Identity Context.
2. Local Bootstrap establishes only missing Local System Rules and required working paths.
3. Local files do not establish independent governance authority.

The Local System Rules Template is pending design.
