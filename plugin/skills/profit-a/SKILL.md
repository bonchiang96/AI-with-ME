---
name: profit-a
description: The AI with ME PROFIT + A Framework for defining AI tasks and Prompts. PROFIT defines the task through Persona, Result, Objective, Feed, Insight and Template. A defines the readiness Acknowledgement for the selected Feed Mode. Use for every Sub-agent Prompt, every Plugin Development Prompt and any AI task or Prompt the user wants defined.
compatibility: Requires the Google Drive and Google Docs connectors through the host. The Plugin does not ship the connectors.
---

# PROFIT + A Framework

## 1. Applicability

1. All Sub-agent Prompts and Plugin Development Prompts use the complete PROFIT + A Framework.
2. Write them in Strict Mode under the [Global Writing Rules](../global-writing-rules/SKILL.md).
3. PROFIT defines the task. A defines the readiness handshake before execution.

## 2. PROFIT elements

Define these six elements:

1. **P — Persona.** Who the AI should be: the necessary role, skills, experience and domain knowledge.
2. **R — Result.** The exact deliverable or outcome the AI should produce.
3. **O — Objective.** Why the task is necessary and what the Result should achieve.
4. **F — Feed.** The source material the AI receives.
   Feed is the material itself: data, documents, images, references, product information, previous outputs or other inputs.
5. **I — Insight.** How to understand the Feed and shape the Result.
   Insight may cover audience, platform, tone, constraints, priorities, research findings, strategic direction or other interpretation.
6. **T — Template.** The final Result's structure, format and presentation.

## 3. Feed Modes

1. **Provide Now.** Include the required Feed with the Prompt.
2. **Provide Later.** Define the required Feed. The user provides it in the next message.
3. **Continuous Feed.** Continue the task across several turns.
   New Feed may extend, change or replace earlier working context.

## 4. Acknowledgement

Acknowledgement is always the final part of the Prompt.
Apply the handshake for the selected Feed Mode:

1. **Provide Now.** The AI confirms readiness. It waits for the user's explicit start signal.
2. **Provide Later.** The AI confirms readiness and states the required Feed. It executes once the Feed arrives.
3. **Continuous Feed.** The AI confirms readiness once at the start or reset point. It then processes later Feed directly.

## 5. Feed In

Feed In is a supporting concept, separate from PROFIT + A.
It defines what the user needs to prepare or provide to use the Prompt.

## 6. Composition

1. Arrange the six PROFIT elements in any order that keeps the final Prompt clear and natural.
2. In the final Prompt, “I” refers to the user and “You” refers to the AI.
3. During Framework review or drafting, describe definitions naturally.
4. Apply I / You wording only when composing the final Prompt.
