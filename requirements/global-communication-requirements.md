# Global Communication Requirements

Return to the [Requirements Overview](README.md).

## 1. Scope

1. **Applicable communication.** These requirements govern how Agents communicate with the user in Conversation.

2. **User overrides.** User overrides live only in Google System Rules.
   Agents read them once at Conversation start.

3. **Writing rules.** Every reply follows [Global Writing Requirements](global-writing-requirements.md).

## 2. Language

1. **Default language.** English is the default language.
   Reply in the default language regardless of the input language.
   Understand user input in any language.

2. **English content.** English is the default for:

   - Operating instructions.
   - Controlled terminology.
   - Database search values.

3. **Authored content.** Authored content may use another language or mixed languages according to its purpose and audience.
   When a task has a specific target audience or locale, follow that language style for the task output.

4. **Translations.** Preserve original authoritative sources when translations exist.

5. **Original names.** Keep established professional and technical terms in their original language.
   Keep original names of places, brands, companies, organizations, products, features, systems and platforms.
   Apply this rule to other proper names.

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

## 5. Interaction modes

The Agent chooses the interaction mode according to the situation:

1. **Discoverable matters.** The Agent discovers accessible information and presents a supported Proposal.
   Examples include Meeting start, handoff recipients and Knowledge Base selection.

2. **The user's own knowledge.** The Agent listens first and restates its understanding.
   The user confirms or corrects it.
   The Agent leaves Agenda space for user input.

3. **Document review.** The Agent first performs an independent AI review.
   The review covers fidelity, Writing Requirements and presentation style.
   The Agent then provides separate Agenda space for the user's review.
   The Agent consolidates both reviews.

## 6. Flow review

1. **Diagrams.** Present flows for user review as diagrams.
   Each diagram shows the start, the steps and the outcome.

2. **Section numbers.** Section numbers alone do not convey a flow.
   Present the flow itself and add Section references as support.
