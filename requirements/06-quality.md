# Quality

Return to the [Requirements Overview](README.md).

## 1. Deliverable quality and independent QA

1. **Actual artifacts.** Every Agent must verify the latest saved version of each Deliverable it creates or modifies.
   Verification of a Working Document does not replace verification of separate Deliverables.

   Final Minutes and other Deliverables require full Content, Writing and Formatting verification.
   Meeting Records require accurate, verified persistence under [Meeting Lifecycle Section 2.4](03-meeting-lifecycle.md#2-discussion-and-outcomes).
   They require neither mandatory [Global Writing Rules](global-writing-rules.md) document QA nor a Quality Checklist.

2. **Three dimensions.** Verify these dimensions separately:

   - Content Quality.
   - Writing Compliance.
   - Formatting Compliance.

   Content includes:

   - Completeness.
   - Correctness.
   - Approved Scope.
   - Source fidelity.

   Information the user provides is certified by the user under [Requirements Overview Section 1.4](README.md#1-framework-definition).
   QA must not mark it FAIL, unverified or Unable to Verify for lack of third-party sources.

   Writing follows active [Global Writing Rules](global-writing-rules.md) and the correct Writing Mode. Formatting follows the artifact format and applicable Operating Guide. Apply output-specific checks required by the assigned role and deliverable.

3. **Self-check steps.** The self-check has two parts: writing checking and save checks.

   Writing checking:

   1. It applies to Final Minutes, Knowledge Bases and text Deliverables, under [Global Writing Rules Section 8](global-writing-rules.md#8-follow-and-checking).
   2. Other outputs follow the Global Writing Rules without separate checking. Examples are Meeting Records, Job Records, Deliverable Guidelines, Identity Context and inbox messages.
   3. It runs on the complete final version before the version is written to Google. In Workspace mode, it runs before the sync.
   4. For Final Minutes and Knowledge Bases, the Parent writes. A new reviewer Sub-agent receives only the final version, its Writing Mode and the Global Writing Rules.
   5. The reviewer checks and enhances the text and replies with feedback. It never translates the content.
   6. The Parent applies feedback about the Global Writing Rules. The Parent ignores feedback that changes the meaning. The Parent makes the final judgment.
   7. One reviewer round is enough.
   8. Without a genuine Sub-agent, the Parent does the checking itself, with the mechanical scan.
   9. Text Deliverables follow the author and reviewer roles under [Execution Lifecycle Section 4](04-execution-lifecycle.md#4-execution-parent-and-sub-agents) and the review rounds of their Workflow.
   10. Non-text Deliverables, such as a website, are outside writing checking.
   11. It includes a language check under [Global Communication Rules Section 2](global-communication-rules.md#2-language). The content keeps its original language, or the content language that an instruction sets under Section 2.4 of those rules. In Final Minutes, each material Decision keeps its User's words. In Knowledge Bases, User's words stay with the knowledge they explain. User's words stay untranslated.

   Rationale: an Agent that checks its own writing tends to record PASS without checking. A reviewer who did not take part in the Meeting reads the text as a reader does.

   Save checks, for every artifact subject to full QA, after it is saved:

   1. Read back the complete saved artifact. A draft in the Conversation is not evidence.
   2. Content: check each Local QA criterion in the artifact's Operating Guide.
   3. Writing: confirm that writing checking ran and that the saved text matches the checked version.
   4. Formatting: check each heading style against the Operating Guide. Check the Easy to Read rule in Section 1.5.
   5. Correct every failure. Read back the saved artifact again.
   6. Record PASS or FAIL for each dimension with the findings. Record PASS only for a check actually performed.

   Every Lifecycle points to these steps. A change to quality checking changes only this Section and the workflow-qa Skill.

   Requirements inspection follows [Requirements Overview Section 2.9](README.md#2-binding-non-functional-requirements).

4. **Formatting checkpoints.** Verify Formatting after creating and saving Job Records and Final Minutes.
   Verify final Formatting again at Protocol completion.
   Routine edits need not each trigger a full Formatting check.
   Meeting Records follow [Section 1.1](#1-deliverable-quality-and-independent-qa).

5. **Easy to Read.** Formatting must provide:

   - Readable hierarchy.
   - Natural information flow.
   - Visual balance.
   - Quick navigation.

   It must help intended readers:

   - Follow the artifact.
   - Understand it.
   - Scan it.

   Apply the rules for whichever artifact format applies:

   - Google Docs.
   - Markdown.
   - Other formats.

6. **Operating Guides.** A Document Operating Guide must own its document's:

   - Purpose.
   - Names.
   - Metadata.
   - Sections.
   - Formatting.
   - Local QA criteria.

   Lifecycle actions and cross-resource execution belong in the Plugin Skills. Apply structural refinements prospectively while preserving historical records and approved formats.
   Placement and standard templates follow [Foundation Section 6](01-foundation.md#6-templates-and-operating-guides).

7. **Writing meaning.** Written outputs must preserve meaning under [Global Writing Rules](global-writing-rules.md).

8. **Writing clarity.** Written outputs must meet the clarity and structure rules in [Global Writing Rules](global-writing-rules.md).

9. **Strict Mode.** Apply Strict Mode to the artifacts that [Global Writing Rules](global-writing-rules.md) assigns to Strict Mode.

10. **Language.** Apply the language rules in [Global Communication Rules](global-communication-rules.md).

11. **Independent QA Workflow.** Independent QA is a normal Workflow.
    The Execution Agent runs it as a Job Scope, usually through a Sub-agent.
    It may be review-only. It may run periodically.
    The user requests a QA Job from the Execution Agent through a Meeting or directly.
    Its assessments and reports must be independent, complete and objective.
    It must inspect every approved item at the authorized depth.
    It may inspect other working Scopes only within specifically approved Job Scope.

    Possible dimensions include:

    - Structure.
    - Operating Guide compliance.
    - Requirement fidelity.
    - Decision-to-Deliverable Fidelity.
    - Context authority.

    Writing Compliance is compulsory for substantively inspected or authored documents subject to full QA under [Section 1.1](#1-deliverable-quality-and-independent-qa).

12. **Fidelity inspection.** Compare full substantive meaning, including:

    - Intent.
    - Requirements.
    - Constraints.
    - Qualifications.
    - Approved revisions.

    Identify:

    - Omissions.
    - Weakening.
    - Excessive editing.
    - Unauthorized additions.
    - Changed requirements.

    Trace the earliest verified divergence and its downstream effect. Source citations alone do not establish fidelity.

13. **QA reporting.** Each inspected item needs:

    - Exact source and target references.
    - Criteria.
    - Evidence.
    - Findings.
    - A result using one of these statuses:
      - PASS.
      - FAIL.
      - Unable to Verify.

    Fidelity findings must identify a useful correction starting point and final impact. Report inadequate evidence without presuming compliance.

14. **Independent QA limits.** Complete every approved audit item without cached PASS reuse or automatic skipping. A review-only QA Job does not edit inspected resources. QA reports identify deficiencies but do not authorize correction. A completed audit may contain failed or unverifiable findings.
