---
name: system-entry
description: Starts every AI with ME Conversation. Checks actual Google Drive and Google Docs access and locates the "AI with me" System Root. Opens System Context, lets the user select a registered Identity and opens its Identity Context and index. Loads the Role Lifecycle. Runs Bootstrap when the System Root is confirmed absent. Use at the start of every Conversation or when the user asks to enter the AI with ME System.
compatibility: Requires the Google Drive and Google Docs connectors through the host. The Plugin does not ship the connectors.
---

# System Entry

## 1. Purpose

This Skill brings each Conversation from its start to a selected, loaded Identity.
The outcome is an Identity ready for NEW MEETING or NEW JOB.

Flow, part 1: access check → locate System Root → open System Context → read System Rules.
Flow, part 2: select Identity → open Identity Context and index → load Role Lifecycle → ready.

## 2. Rules for every reply

1. Apply the [Global Communication Rules](../../rules/global-communication-rules.md).
2. Apply the [Global Writing Rules](../../rules/global-writing-rules.md).
3. Read these rule files from the Plugin, not from Google Drive.
4. System Rules take priority over the Plugin. Apply the System Rules of the actual environment.
5. When an arrangement is undecided, show it to the user as undecided. Do not invent governance.

## 3. Access check

1. Check actual Google Drive and Google Docs access for the action you need.
2. A connected tool name does not prove access. Confirm access by a real read.
3. Google Drive / Docs is the authority for governance, records, indexes and inbox messages.
4. When a connector, capability or permission is unavailable, explain the practical limitation to the user.
5. Discuss the next authorized step.
6. Perform or guide permitted setup within your capabilities.
7. Do not claim that an incomplete action succeeded.

Missing Google access limits governed work. It never blocks installation of the Plugin.
Access restoration is left to your judgment within authorized Scope.

## 4. Entry flow

1. Locate the central Google Drive folder named “AI with me”.
2. Open System Context in that folder.
3. Assess access to the applicable System Rules.
4. Read the user overrides in the applicable System Rules once.
5. Reuse existing accessible resources.
6. Present the active registered Identities from System Context.
7. The user selects one Identity.
8. Open the Identity's 00 Identity Context and 01 Index through its registered identity folder.
9. Load the Skill for that Identity's Role:
   - Meeting Agent: [meeting-agent](../meeting-agent/SKILL.md).
   - Execution Agent: [execution-agent](../execution-agent/SKILL.md).
10. Load applicable System Rules and Plugin Skills for the assignment.
11. Discover current information before asking the user for it again.

The Identity is then ready for NEW MEETING or NEW JOB.
These four words are the user's stage words. Each Role Skill holds the flow of its stages.

## 5. Identity resolution

1. Accept a directly supplied Identity Context Locator or a registered Identity resolved through System Context.
2. Both paths must reach the Identity Context through the identity folder.
3. A Google Locator is the Google Docs link of a file. For a Tab, it is the Tab link.
4. Resolve the user's assignment against registered Scope information.
5. Resolve a missing or ambiguous Identity before scoped Messaging.
6. Do not default an unresolved scoped assignment to another Identity.
7. Inactive or archived Identities are excluded from normal active choices.
8. An inactive or archived Identity may be reactivated when appropriate.

## 6. Bootstrap

Bootstrap runs only when the System Root is confirmed absent.

1. Inaccessibility alone does not prove absence.
2. Resolve access or location uncertainty before creating another Root.
3. The General Meeting Agent holds the Bootstrap Meeting under the [meeting-agent](../meeting-agent/SKILL.md) Lifecycle.
4. It uses the Agent Key `general-meeting` from the start.
5. It needs no Registry entry until Bootstrap registers it.
6. Bootstrap records remain in the Conversation until the folder exists.

In the Meeting, explain the proposed:

- Root.
- System Context.
- System Rules.
- Knowledge Base folder.
- Responsibilities.
- Minimum Identities.
- Creation actions.

The user approves the System arrangement and its creation actions in that Meeting.
After CLOSE MEETING, the General Meeting Agent performs these Post-Meeting Actions:

1. Create the folder.
2. Create System Context from the [System Context](../../templates/system-context.md) template.
3. Create Google System Rules from the [Google System Rules](../../templates/system-rules.md) template, with its starter rules.
4. Create the Knowledge Base folder with its [00 Index](../../templates/knowledge-base-index.md) and [general Knowledge Base](../../templates/general-knowledge-base.md).
5. Establish the two minimum Identities under the Identity setup in [meeting-agent](../meeting-agent/SKILL.md):
   - The General Meeting Agent, with Agent Key `general-meeting`.
   - The General Execution Agent, with Agent Key `general-execution`.
6. Save the Bootstrap Working Record and Final Minutes as the System's first records.
7. Join the normal entry flow at Identity selection.

Restore genuinely missing resources within existing approved authority and applicable System Rules.

## 7. Local environments

Local working is hybrid. Google Drive remains the authority.

1. Local environments use the central System Root, System Context and Identity Context.
2. System Context, Identity Context, the index and the inbox always stay in Google.
3. Local Bootstrap establishes only missing Local System Rules and required working paths.
4. Local System Rules define the local folder, its arrangement, and when and how work returns to Google.
   They reside in Chapter 4 of [Google System Rules](../../templates/system-rules.md#4-local-system-rules).
5. The local root holds one folder per Identity, named by its Agent Key.
6. Each Identity folder holds one folder per Meeting or Job, named like its Google Tab.
7. Local files do not establish independent governance authority.
