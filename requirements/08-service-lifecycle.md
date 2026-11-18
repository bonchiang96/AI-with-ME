# Service Lifecycle

Return to the [Requirements Overview](README.md).

## 1. Role and setup

1. **Role.** A Service Agent runs schedule-triggered or event-triggered work for one Meeting Identity.
   That Identity is its governing Meeting Agent.
   The Service Lifecycle follows the [Execution Lifecycle](04-execution-lifecycle.md) with these differences:

   - No person approves the Execution Plan.
   - It sends no Completion Notice.
   - It has no inbox and reads no inbox.

   No person attends a run. The Service Agent must not ask the user a question or wait for an answer.

2. **Setup owner.** The governing Meeting Agent sets up a Service Agent Identity for its own Scope.
   It defines the Service Guideline with the user in a Meeting.
   After CLOSE MEETING, it performs the setup as Post-Meeting Actions:

   1. Create the identity folder with 00 Identity Context, 01 Index and 02 Job Records.
   2. Write the Service Guideline in the 00 Identity Context.
   3. State the run log Tab arrangement in the 01 Index Operating Guide.
   4. Register the Identity in System Context under [Section 1.4](#1-role-and-setup).
   5. Create the scheduled task that triggers each run.
      When the Meeting Agent cannot create it, it arranges the step with the user.

3. **Service Guideline.** The Service Guideline is a Chapter of the Service Agent's 00 Identity Context.
   The Service Agent reads no other file for its rules.
   The Service Guideline must state:

   - The Scope.
   - How to retrieve the data before intake.
   - How to analyze and judge the data.
   - The intake requirements.
   - The Execution Plans and how to choose one for each item.
   - The fallback plan.
   - How to assign Sub-agents.
   - What to record at the end of a Job.
   - Whether to notify the user, and through which channel.

   A fallback plan is always required.
   The governing Meeting Agent decides how to group the Execution Plans.
   A change to the Service Guideline applies from the next run.

4. **Registration.** A Service Agent Identity is registered in System Context with the five Registry fields.
   Its Role is Service Agent.
   Its Responsibility and Scope begins with the Meeting Identity it serves.
   The governing Meeting Agent registers it. This authority covers only a Service Agent for its own Scope.
   When the Status becomes Inactive or Archived, the governing Meeting Agent stops or removes the scheduled task.

5. **Entry.** The Identity selection list must not show Service Agent Identities.
   A run started by a trigger names its Agent Key. Entry selects that Identity without asking the user.
   The governing Meeting Agent triggers a test run. The user does not enter a Service Agent Identity by hand.

6. **High-volume events.** Work with many parallel requests must use batch processing.
   Separate code receives the requests and stores them.
   The Service Agent processes the stored requests on a schedule.
   One Job then holds many items, and each item has its own status.
   The governing Meeting Agent may arrange a small application that receives the requests.
   It gives the Service Agent an MCP server or a command line tool to read them.

## 2. Run

1. **Shared forward flow.** Each run must use this sequence:

   1. Read the Service Guideline.
   2. Intake.
   3. Execution Plan.
   4. Proceed gate.
   5. Execution.
   6. Recording.

   Each run is a new Conversation.

2. **Intake.** The Service Agent retrieves the data, analyzes it and checks every intake requirement.
   Intake ends with exactly one outcome:

   - Idle: nothing needs processing. This outcome is normal.
   - Blocked: work exists, but an intake requirement is not met.
   - Executed: intake passed and the work starts.

   Blocked concerns the whole run, not single items.
   An idle or blocked run adds its run log row and stops. It opens no Job.

3. **Execution Plan.** For each item, the Service Agent judges the data and finds the fitting Execution Plan in the Service Guideline.
   An item with no fitting Execution Plan follows the fallback plan.
   The Service Agent must save the Execution Plan in the Job Record before execution.

4. **Proceed gate.** The proceed gate replaces PROCEED EXECUTION. No person approves it.
   It passes when intake ended as executed and the Execution Plan is saved.

5. **Execution.** The Service Agent performs only the work that the Service Guideline authorizes.
   It runs the tasks of the Plan through Sub-agents where the environment allows.
   The Parent coordinates and performs a task itself only when a Sub-agent cannot.
   Each item has its own status.

6. **Fallback.** The Service Agent follows the fallback plan when no Execution Plan fits an item or execution meets any problem.
   It records the item as fallback with the reason.
   It hands the Job back with one Information row in the governing Meeting Agent's inbox.
   The row links the Job Record.

## 3. Records

1. **Run log.** The 01 Index of a Service Agent is its run log.
   Every run adds exactly one row with:

   - Time.
   - Status: idle, blocked or executed.
   - Description.
   - Job: the Job key, only for executed.

   The governing Meeting Agent decides the Tab arrangement.

2. **Job Record.** Each Job has one Tab in the 02 Job Records file.
   The Tab name holds the date, the time and the Job key, without a status.
   A Service Job key uses S and a number in sequence.
   The Parent records every report and every valuable result when it returns, under [Execution Lifecycle Section 5.8](04-execution-lifecycle.md#5-job-record).
   The Parent consolidates every result into one complete Job Record after execution.
   After the completion sync, the Parent cleans the Job's workspace folder under [Environments and Acceptance Section 2.16](07-environments-and-acceptance.md#2-hybrid-local-working-and-deliverable-storage).
   A Service Job needs no other index row.

3. **Review.** The governing Meeting Agent learns the outcome of the runs by reading the run log and the Job Records.
   It reads them when the user asks.
   The Service Agent sends no notice for a normal run.

4. **Cleaning.** The governing Meeting Agent owns cleaning of the run log and the Job Records.
   It decides how long to keep the run log Tabs. All Job Records are kept for now.
   It may first conclude a period into a report and then clean the records of that period.
   The Service Agent must not clean or remove any record in Google. Workspace cleanup removes local files only.
