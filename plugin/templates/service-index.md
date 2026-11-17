# 01 Index

## Tab 1. Operating Guide

1. **Purpose.** The index of a Service Agent is its run log.
   Every run adds exactly one row, whether or not it executes a Job.
   The run log shows which runs happened, which executed and why a run did not execute.

2. **Names.** The file name is 01 Index.
   It resides in the Service Agent's identity folder.

3. **Metadata.** The file needs no metadata beyond its title.

4. **Sections.** This Operating Guide is the first Tab. The run log Tabs follow it.
   The governing Meeting Agent states the Tab arrangement in item 7.
   Examples are one Tab for each day, or one Tab for all runs.

5. **Formatting.** Use a Google Docs file with a native table in each run log Tab.
   Each row has four fields:

   1. Time: the run time in the Google System Rules date and time format.
   2. Status: idle, blocked or executed.
   3. Description.
   4. Job: the Job key, only for executed.

   The Status values mean:

   - idle: nothing needed processing. This outcome is normal.
   - blocked: work existed, but an intake requirement was not met. The Description names the requirement.
   - executed: intake passed and a Job ran. The Description states what the Job processed.

   Blocked concerns the whole run, not single items.
   Each item's status belongs in the Job Record.
   A Service Job key uses S and a number in sequence, such as S-0001.

6. **Local QA criteria.** Check these points after each new row:

   1. The run has exactly one row.
   2. The Status is one of the three values.
   3. A blocked row names the requirement that was not met.
   4. An executed row holds the Job key of an existing Job Record Tab.

7. **Tab arrangement and cleaning.** The governing Meeting Agent states here:

   - How the run log Tabs are arranged.
   - How long the run log Tabs are kept.

   The governing Meeting Agent cleans the run log. The Service Agent removes nothing.

## Run log Tab

| Time | Status | Description | Job |
| --- | --- | --- | --- |
