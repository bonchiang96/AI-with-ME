# System Rules

## 1. Operating Guide

1. **Purpose.** System Rules express user-defined shared operating conventions for one execution environment.
   Agents apply the rules for the actual execution environment.
   Applicable System Rules override conflicting Plugin instructions for the environment operations they govern.

2. **Names.** Name the file after its environment, such as Google System Rules or Local System Rules.
   Google System Rules reside in the System Root.

3. **Metadata.** The file needs no metadata beyond its title and environment.

4. **Sections.** The file has these Chapters:

   1. Operating Guide.
   2. Environment Rules.
   3. Synchronization.
   4. User Communication Overrides.

   The detailed Google and Local System Rules Templates are pending design.

5. **Formatting.** Use a Google Docs file for Google System Rules.
   Use numbered rules.
   Keep one rule per point.

6. **Local QA criteria.** Check these points after each change:

   1. Each rule is a user-defined convention.
   2. Each rule belongs to the Chapter that owns its meaning.
   3. The file holds only current truth.

## 2. Environment Rules

Google System Rules govern Google-side:

- Document creation.
- Locations and storage structure.
- Resource maintenance.

Local System Rules govern:

- Local file formats.
- Naming.
- Directories and working paths.
- Local Record creation.
- Local Deliverable creation.
- Which outputs synchronize to Google.

(Rules: pending design.)

## 3. Synchronization

Synchronization order and timing.

(Rules: pending design.)

## 4. User Communication Overrides

User overrides of the Global Communication Rules.
Agents read them once at Conversation start.

(Overrides: none.)
