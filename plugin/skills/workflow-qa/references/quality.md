# Quality

## 1. Deliverable quality and independent QA

1. **Actual artifacts.** Every Agent must verify the latest saved version of each Deliverable it creates or modifies.
   Verification of a Working Document does not replace verification of separate Deliverables.

   Final Minutes and other Deliverables require full Content, Writing and Formatting verification.
   Meeting Working Records require accurate, verified persistence under [Meeting Lifecycle Section 2.4](../../meeting-agent/references/lifecycle.md#2-discussion-and-outcomes).
   They require neither mandatory [Global Writing Rules](../../../rules/global-writing-rules.md) document QA nor a Quality Checklist.

2. **Three dimensions.** Verify these dimensions separately:

   - Content Quality.
   - Writing Compliance.
   - Formatting Compliance.

   Content includes:

   - Completeness.
   - Correctness.
   - Approved Scope.
   - Source fidelity.

   Writing follows active [Global Writing Rules](../../../rules/global-writing-rules.md) and the correct Writing Mode. Formatting follows the artifact format and applicable Operating Guide. Apply output-specific checks required by the assigned role and deliverable.

3. **Evidence.** For every artifact subject to full QA, record actual PASS or FAIL for each affected dimension.
   Record permitted corrections and successful verification of the latest saved version.
   Read the complete final artifact after substantive changes before claiming compliance.

   Requirements inspection follows [Requirements Overview Section 2.9](../../system-entry/references/principles.md#2-binding-non-functional-requirements).

4. **Formatting checkpoints.** Verify Formatting after creating and saving Job Records and Final Minutes.
   Verify final Formatting again at Protocol completion.
   Routine edits need not each trigger a full Formatting check.
   Meeting Working Records follow [Section 1.1](#1-deliverable-quality-and-independent-qa).

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

   Lifecycle actions and cross-resource execution belong in Commands. Apply structural refinements prospectively while preserving historical records and approved formats.
   Placement and standard templates follow [Foundation Section 6](../../system-entry/references/foundation.md#6-templates-and-operating-guides).

7. **Writing meaning.** Written outputs must preserve meaning under [Global Writing Rules](../../../rules/global-writing-rules.md).

8. **Writing clarity.** Written outputs must meet the clarity and structure rules in [Global Writing Rules](../../../rules/global-writing-rules.md).

9. **Strict Mode.** Apply Strict Mode to the artifacts that [Global Writing Rules](../../../rules/global-writing-rules.md) assigns to Strict Mode.

10. **Language.** Apply the language rules in [Global Communication Rules](../../../rules/global-communication-rules.md).

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
