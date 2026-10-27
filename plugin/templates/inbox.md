# 02 Inbox

## 1. Operating Guide

1. **Purpose.** Hold Work Requests and Completion Notices routed to this exact registered Identity.
2. **Name.** Use **02 Inbox** as a Google Docs file in the identity folder.
3. **Metadata.** Identify the recipient's exact Agent Key.
4. **Chapters.** Keep this guide first and the inbox table next.
5. **Formatting.** Use a native Google Docs table with the five columns below.
6. **Local QA.** Verify exact recipient, sender Identity, message Type, closed-record Ref and meaningful source relationships.
   Apply [Writing Rules](../rules/global-writing-rules.md) Strict Mode to messages.

The [Inbox skill](../skills/inbox/SKILL.md) owns reading, processing, sending and verification actions.
Sent holds the actual sending time. From names the sender Identity.
Ref names the closed record key in the sender's index.

## 2. Inbox

| Sent | From | Type | Ref | Message |
| --- | --- | --- | --- | --- |
| {{actual local time}} | {{sender Identity}} | {{Work Request or Completion Notice}} | {{sender's closed-record key}} | {{bounded request or verified outcome with references}} |
