# Google System Rules

## 1. Operating Guide

1. **Purpose.** Google System Rules express the user's shared operating conventions for the Google environment.
   They govern Google-side document creation, locations and storage structure, and resource maintenance.
   Chapter 4 holds the Local System Rules for local working.
   System Rules take priority over the Plugin.

2. **Names.** The file name is Google System Rules.
   It resides in the System Root, the Google Drive folder named “AI with me”.

3. **Metadata.** The file needs no metadata beyond its title.

4. **Sections.** The file has these Chapters:

   1. Operating Guide.
   2. Google Rules.
   3. User Communication Overrides.
   4. Local System Rules.

   Chapter 2 starts with the starter rules. The user may add rules, such as a further inbox Type.
   Chapter 3 holds user overrides of the Global Communication Rules. Agents read them once at Conversation start.
   Chapter 4 starts with the decided local rules.
   Local Bootstrap adds the local root path and other local rules to Chapter 4, following Environments and Acceptance Section 2.2.

5. **Formatting.** Use a Google Docs file.
   Use numbered rules.
   Keep one rule per point.

6. **Local QA criteria.** Check these points after each change:

   1. Each rule is a user-defined convention.
   2. Each rule belongs to the Chapter that owns its meaning.
   3. The file holds only current truth.

## 2. Google Rules

1. **Documents.** Create documents as Google Docs. Use native tables for tables.
2. **Tab names.** Name each Tab with the pattern date — Topic — key.
   An example is 2026-10-27 — Plugin Build — J-0256.
3. **Date and time.** Write each date and time as YYYY-MM-DD HH:MM in 24-hour time.
   Add the time-zone abbreviation. An example is 2026-10-27 19:45 MYT.

## 3. User Communication Overrides

## 4. Local System Rules

1. **Local folder arrangement.** The local root holds one folder per Identity, named by its Agent Key.
   Each Identity folder holds one folder per Meeting or Job.
   Name each Meeting or Job folder like its Google Tab.
2. **Google-only resources.** Keep System Context, Identity Context, the index and the inbox in Google.
3. **Record return.** Return the Working Record and Final Minutes to Google at Meeting close.
   Return the Job Record to Google at Job completion.
4. **Indexing and announcement.** Index or announce work only after its record is in Google.
   Its Deliverable must also be in the agreed storage place.
