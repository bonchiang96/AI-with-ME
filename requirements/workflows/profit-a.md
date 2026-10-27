# PROFIT + A Framework

Return to the [Requirements Overview](../README.md).

## 1. PROFIT + A Framework

1. **Framework purpose.** PROFIT + A must provide a reusable Framework for defining AI tasks and Prompts.
   PROFIT defines the task. A defines the readiness handshake before execution.

2. **Prompt applicability.** All Sub-agent Prompts and future Plugin Development Prompts must use the complete PROFIT + A Framework.
   Apply Strict Mode under [Global Writing Rules](../global-writing-rules.md).

3. **PROFIT elements.** Define these six elements for the task:

   1. **P — Persona.** Define who the AI should be for the task, including the necessary:
      - Role.
      - Skills.
      - Experience.
      - Domain knowledge.
   2. **R — Result.** Define the exact deliverable or outcome the AI should produce.
   3. **O — Objective.** Define why the task is necessary and what the Result should achieve.
   4. **F — Feed.** Identify the source material the AI receives to perform the task.
      Feed is the material itself. It may include:
      - Data.
      - Documents.
      - Images.
      - References.
      - Product information.
      - Previous outputs.
      - Other inputs.
   5. **I — Insight.** Define how the Feed should be understood and how the Result should be shaped.
      Insight may include:
      - Audience.
      - Platform.
      - Tone.
      - Constraints.
      - Priorities.
      - Research findings.
      - Strategic direction.
      - Other interpretation.
   6. **T — Template.** Define the final Result's:
      - Structure.
      - Format.
      - Presentation.

4. **Feed Modes.** Use the applicable mode:

   1. **Provide Now.** Include the required Feed with the Prompt.
   2. **Provide Later.** Define the required Feed. The user provides it in the next message.
   3. **Continuous Feed.** Continue the task across multiple turns.
      New Feed may affect earlier working context through:
      - Additions.
      - Changes.
      - Replacement.

5. **Acknowledgement.** Acknowledgement must remain the final part of the Prompt.
   Apply the readiness handshake for the selected Feed Mode:

   1. **Provide Now.** The AI confirms readiness. It waits for the user's explicit start signal before execution.
   2. **Provide Later.** The AI performs these steps:
      1. Confirm readiness.
      2. State the required Feed.
      3. Execute once that Feed is provided.
   3. **Continuous Feed.** The AI confirms readiness once at the start or reset point.
      It then processes subsequent Feed directly.

6. **Feed In.** Feed In is a supporting concept, separate from PROFIT + A.
   It defines what the user needs to prepare or provide to use the Prompt.

7. **Prompt composition.** Arrange the six PROFIT elements in any order that makes the final Prompt clear and natural.
   In the final Prompt:

   - I refers to the user.
   - You refers to the AI.

   During Framework review or drafting, describe definitions naturally.
   Do not force I / You wording before composing the final Prompt.
