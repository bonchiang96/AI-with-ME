---
name: ai-with-me
description: Starts every AI with ME Conversation. Checks actual Google Drive and Google Docs access and locates the "AI with me" System Root. Opens System Context, lets the user select a registered Identity and opens its Identity Context and index. Loads the Role Lifecycle. Runs Bootstrap when the System Root is confirmed absent. Use at the start of every Conversation or when the user asks to enter the AI with ME System.
compatibility: Requires the Google Drive and Google Docs connectors through the host. The Plugin does not ship the connectors.
---

# AI with ME — System entry

## 1. Purpose

This Skill brings each Conversation from its start to a selected, loaded Identity.
The outcome is an Identity ready for NEW MEETING or NEW JOB.

Flow, part 1: access check → locate System Root → open System Context → read System Rules.
Flow, part 2: select Identity → open Identity Context and index → load Role Lifecycle → ready.

## 2. Rules for every reply

1. Use the [global-communication-rules](../global-communication-rules/SKILL.md) Skill for every reply.
2. Use the [global-writing-rules](../global-writing-rules/SKILL.md) Skill for every output.
3. Load both as Plugin Skills. Do not read them from Google Drive.
4. System Rules take priority over the Plugin. Apply the System Rules of the actual environment.
5. When an arrangement is undecided, show it to the user as undecided. Do not invent governance.

## 3. User authority

The user is the only authority who certifies the information the user provides.
This applies to every Identity and every judgment.

1. Accept the user's information fully, including what the user remembers or believes.
2. Record it faithfully as the user stated it.
3. Use it as the working truth and continue the work with it.
   Do not doubt it, mark it unverified, label it an assumption or hold it pending verification.
   Do not block or delay work to wait for outside confirmation.
4. Do not require third-party verification or sources for it.
5. For a legal matter, such as a product registration, you may also check official sources yourself.
   Report the result to the user without doubting the user.

## 4. Access check

1. Check actual Google Drive and Google Docs access for the action you need.
2. A connected tool name does not prove access. Confirm access by a real read.
3. Google Drive / Docs is the authority for governance, records, indexes and inbox messages.
4. When a connector, capability or permission is unavailable, explain the practical limitation to the user.
5. Discuss the next authorized step.
6. Perform or guide permitted setup within your capabilities.
7. Do not claim that an incomplete action succeeded.

Missing Google access limits governed work. It never blocks installation of the Plugin.
Access restoration is left to your judgment within authorized Scope.

## 5. Entry flow

1. Locate the central Google Drive folder named “AI with me”.
2. Open System Context in that folder.
3. Assess access to the applicable System Rules.
4. Read the user overrides in the applicable System Rules once.
5. Reuse existing accessible resources.
6. Present the registered Identities with Status Active from System Context.
7. The user selects one Identity.
8. Open the Identity's 00 Identity Context and 01 Index through its registered identity folder.
9. Check the Agent workspace under Section 8.1. State the working mode to the user.
10. Load the Skill for that Identity's Role:
   - Meeting Agent: [meeting-agent](../meeting-agent/SKILL.md).
   - Execution Agent: [execution-agent](../execution-agent/SKILL.md).
11. Load applicable System Rules and Plugin Skills for the assignment.
12. Discover current information before asking the user for it again.

The Identity is then ready for NEW MEETING or NEW JOB.

One Conversation serves one Identity.
After the user selects an Identity, the Conversation keeps that Identity until it ends.
Do not switch to another Identity in the same Conversation.
When the user asks to work as another Identity, ask the user to start a new Conversation.

These four words are the user's stage words. Each Role Skill holds the flow of its stages.

## 6. Identity resolution

1. Accept a directly supplied Identity Context Locator or a registered Identity resolved through System Context.
2. Both paths must reach the Identity Context through the identity folder.
3. A Google Locator is the Google Docs link of a file. For a Tab, it is the Tab link.
4. Resolve the user's assignment against registered Scope information.
5. Resolve a missing or ambiguous Identity before scoped Messaging.
6. Do not default an unresolved scoped assignment to another Identity.
7. Inactive or archived Identities are excluded from normal active choices.
8. An inactive or archived Identity may be reactivated when appropriate.
9. The user changes a Status in a Meeting with the General Meeting Agent. Its records stay unchanged.
10. The General Meeting Agent is the Identity named in the System Context Governance Chapter.
    It owns System Governance, Identity definition and registration, and Handoff coordination.
    At Bootstrap it is `general-meeting`. The user may name another Identity in a Meeting with the current General Meeting Agent.

## 7. Bootstrap

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
   Name `general-meeting` in its Governance Chapter.
3. Create Google System Rules from the [Google System Rules](../../templates/system-rules.md) template, with its starter rules.
4. Create the Knowledge Base folder with its [00 Index](../../templates/knowledge-base-index.md) and [general Knowledge Base](../../templates/general-knowledge-base.md).
5. Establish the two minimum Identities under the Identity setup in [meeting-agent](../meeting-agent/SKILL.md):
   - The General Meeting Agent, with Agent Key `general-meeting`.
   - The General Execution Agent, with Agent Key `general-execution`.
6. Save the Bootstrap Meeting Record and Final Minutes as the System's first records.
7. Join the normal entry flow at Identity selection. Only `general-meeting` continues in this Conversation.

Restore genuinely missing resources within existing approved authority and applicable System Rules.

## 8. Agent workspace

An Agent workspace is a file system the Agent can write to, in the cloud or on the user's device.
Google Drive remains the authority.

### 8.1 Workspace check

1. At entry step 9, the Agent judges by itself whether it has a workspace.
2. It may confirm by writing a file.
3. With a workspace, the Agent must use it for the working records in Section 8.2.
4. Without a workspace, the Agent works in the Google style. It writes every record directly to Google.
5. The Agent states the working mode to the user in one line:
   - Workspace mode, with the workspace path.
   - Google mode.
6. The workspace root is `~/ai-with-me/`. Each Identity has one folder there, named by its Agent Key.
   Each Meeting or Job has one folder inside it, named like its Google Tab.
7. When `~/ai-with-me/` is not writable, choose another persistent path and state it to the user.
8. Never use a temporary folder as the workspace, such as `/tmp` or a session scratch folder.
   Rationale: the host may delete a temporary folder at any time, and the working records with it.

### 8.2 Workspace content

1. Only working records go into the workspace:
   - The Meeting Record of a Meeting Agent.
   - The Job Record of an Execution Agent.
   - The Final Minutes draft of a Meeting Agent.
2. Every other resource stays in Google.
   Examples are System Context, Identity Context, the 01 Index, the inbox and Knowledge Bases.
3. Rationale: working records take the most writes.
   Keeping them in the workspace removes most Google writes and the Google output from the Conversation.

### 8.3 Entry record

1. At Opening or record establishment, create the entry record in Google first.
2. The entry record is the record's Tab with only the Meeting Information or the Job metadata.
3. Then create the working file in the workspace. State its path to the user.
4. Write every further change in the workspace until a sync.

### 8.4 Sync

1. **Hard rule.** Sync at Meeting close and at Job completion.
2. **Agent judgment.** Between them, the Agent judges by itself when to sync.
   Reasons include long content, the container lifetime and a risk of disposal.
   No fixed trigger applies, such as each Agenda item.
3. **User command.** SYNC ME is the user's signal for a manual sync. The bare word sync is not a command.
4. **Performer.** When the Agent can use a Sub-agent, a Sub-agent performs the sync.
   The Sub-agent uses the cheapest model available. Otherwise the Agent performs the sync itself.
5. **Check.** The performer of every sync does a readback in Google. The readback checks in this order:
   1. The content is complete and correct.
   2. The heading styles are correct.
6. **Completion sync.** At Meeting close and at Job completion, the records are final and the Final Minutes exist.
   After the Sub-agent's readback, the Agent does its own readback and confirms the result.
7. **Interim sync.** A sync between them needs only the Sub-agent's readback. The Agent does no readback.
   Rationale: only the completion sync makes the Google record final. A second readback in between costs time and tokens.
8. **Failure.** The Agent handles a sync failure itself.

### 8.5 Active record from another Conversation

1. An active record follows the normal continuation flow.
2. When the active record holds only its entry record, ask the user softly whether the work runs in another Conversation.
   - No: continue here.
   - Yes: the user continues in that Conversation.
   - That Conversation cannot continue: the user chooses to restart or to continue from what Google holds.
3. This step is a user choice, not failure handling.

### 8.6 Local device workspace

1. Local System Rules define the local folder and its arrangement.
   They reside in Chapter 4 of [Google System Rules](../../templates/system-rules.md#4-local-system-rules).
2. The local root holds one folder per Identity, named by its Agent Key.
3. Each Identity folder holds one folder per Meeting or Job, named like its Google Tab.
4. Workspace files do not establish independent governance authority.
