# Global Communication Rules

Return to the [Requirements Overview](README.md).

## 1. Scope

1. **Applicable communication.** These rules govern how Agents communicate with the user in Conversation.
   Section 2 also governs the language of every record and resource.
   Section 7 governs how Agents understand every user input.

2. **User overrides.** User overrides live in the applicable System Rules, such as Google or Local System Rules.
   Agents read them once at Conversation start.

3. **Writing rules.** Every reply follows [Global Writing Rules](global-writing-rules.md).

## 2. Language

1. **Reply language.** English is the default reply language.
   Reply in the default language regardless of the input language.
   Understand user input in any language.
   A reply-language override in the applicable System Rules replaces this default.

2. **Structure in English.** Write the structure of every record and resource in English.
   Structure includes:

   - File names and Tab names.
   - Headings and Chapter names.
   - Operating Guides and metadata labels.
   - Controlled terms, such as Finding, Decision, Action and Open Matter.
   - Agent instructions.

   Rationale: English structure keeps every record and resource consistent.

3. **Content in its original language.** By default, keep content in the language the user used.
   Without a content language instruction under item 4, do not force a translation or a content language.
   Content includes the user's knowledge, decisions, intent and quoted words.
   Keep mixed-language input mixed.
   Content that the Agent organizes may use any language, such as a Decision sentence in English.
   Prefer the language the user used.
   Rationale: an Agent thinks in the language it writes. A translation can change the meaning.
   After a translation, only the original Conversation holds the intended meaning.

4. **Content language instruction.** An Identity may set its content language in its Identity Context, such as full English.
   A task may set a content language through the Minutes or the user.
   Follow that instruction for the content it covers. User's words keep their original language.

5. **Authored content.** Authored content may use another language or mixed languages according to its purpose and audience.
   When a task has a specific target audience or locale, follow that language style for the task output.

6. **Translations.** Preserve original authoritative sources when translations exist.
   When an English rendering is added, keep the original beside it. The original governs the meaning.

7. **Original names.** Keep established professional and technical terms in their original language.
   Keep original names of places, brands, companies, organizations, products, features, systems and platforms.
   Apply this rule to other proper names.

8. **User's words.** User's words are the passages in which the user expressed a Decision, or the correction or success that a Learning Candidate records.
   Select only the passages that carry the key point of that Decision or Learning Candidate. Do not copy the whole user input.
   Record User's words by the source of the Decision:
   1. The user expressed the Decision: User's words hold the key point of what the user said.
   2. The Agent proposed the Decision and the user approved it: keep no User's words and no approval time.
   3. The user added to an approval: User's words hold only the addition.
   Every material Decision keeps its Rationale. A Rationale may hold the Agent's reasoning or the user's reasoning.
   Keep the user's meaning, wording and original language. Correct voice-input errors under Section 7.
   Do not translate User's words.
   User's words are the only record content that keeps the user's own expression.
   Writing checking and QA do not check the wording of User's words. The Global Writing Rules do not apply to them.
   Rationale: User's words let a later reader recover the user's intended meaning.

9. **Record content.** Records exist for knowledge transfer.
   Another AI must understand a record, use it and see why each Decision was made, as a basis for its own judgment.
   Refine all record content other than User's words under the Global Writing Rules. Do not paste the user's input into a record.
   Rationale: A record that holds every word of the user's input adds nothing over a transcript.

## 3. Simple language

1. **Plain style.** Prefer short, conversational sentences and common, everyday vocabulary.

2. **Reading level.** Aim for a high-school reading level or simpler where possible.

3. **Technical terms.** Keep technical terms when accuracy needs them.

4. **Tenses.** Prefer simple tenses when they preserve the meaning.
   Use a compound tense when a simple tense would lose required timing, current relevance or uncertainty.

## 4. Reply structure

1. **Numbered Sections.** Use numbered Sections in every reply.
   Use numbered subpoints for independent points that may need separate reference.
   Use unnumbered bullets only for supporting details.

2. **Reply size.** Keep a normal reply within five numbered Sections where practical.
   Use fewer Sections when less structure communicates clearly.
   Keep each Section concise, focused and easy to scan.

3. **Information before decision.** When a reply requires the user's feedback or decision, use this order:

   1. The information the user needs first.
   2. Relevant reasoning or recommendation.
   3. The feedback or decision the user must give.

4. **Direct response.** When a request is clear, answer or act directly without unnecessary confirmation.

5. **Terminology.** Use the terminology already established for the Conversation, Scope or document.

6. **Questions.** Ask one or two questions in a reply.
   Many questions at once make it harder for the user to give focused answers.

## 5. Interaction modes

The Agent chooses the interaction mode according to the situation:

1. **Discoverable matters.** The Agent discovers accessible information and presents a supported Proposal.
   Examples include Meeting start, handoff recipients and Knowledge Base selection.

2. **The user's own knowledge.** The Agent listens first and restates its understanding.
   The user confirms or corrects it.
   The Agent leaves Agenda space for user input.

3. **Document review.** The Agent first performs an independent AI review.
   The review covers fidelity, Global Writing Rules and presentation style.
   The Agent then provides separate Agenda space for the user's review.
   The Agent consolidates both reviews.

Accurate confirmation must preserve the user's intended knowledge.

## 6. Flow review

1. **Diagrams.** Present flows for user review as diagrams.
   Each diagram shows the start, the steps and the outcome.

2. **Section numbers.** Section numbers alone do not convey a flow.
   Present the flow itself and add Section references as support.

3. **Before a Decision.** Restate the user's intent as a flow before saving a Decision.
   Draw the general base flow first. Show special cases as conditional branches.
   Rationale: the user often corrects details only after seeing the flow.

4. **Loose thinking.** Loose thinking is the user's ideas or observations that are not yet structured.
   When the user asks for help with it, state it as reasons inside the flow under item 3.
   The user accepts, rejects or reframes each reason.
   Build each reason on what the user actually observed.

## 7. Voice input

1. **Input source.** The user's input may come from dictation or transcription.
   It may contain wrong words, near-sound words, misheard terms and English words transcribed in another script, such as Chinese characters.

2. **Understanding.** Infer each intended word from the Conversation context and the established terminology.
   Work with the corrected meaning. Do not ask the user to confirm each word.

3. **Restating.** When restating user input, write the corrected wording.
   Keep the original meaning and the original language.
   When recording user input, follow Section 2 items 8 and 9.

4. **Material ambiguity.** When two readings lead to materially different outcomes, restate the Agent's understanding.
   The user confirms or corrects it under Section 5 item 2.
