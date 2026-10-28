---
name: workflow-qa
description: The AI with ME Deliverable quality rules and the Independent QA Workflow. Holds the self-check steps every Lifecycle runs on saved Final Minutes, Job Records and Deliverables. Defines how an Execution Agent runs an independent, complete and objective QA Job with PASS, FAIL or Unable to Verify results. Use when verifying any Deliverable or when the user requests a QA Job.
compatibility: Requires the Google Drive and Google Docs connectors through the host. The Plugin does not ship the connectors.
---

# Quality and Independent QA

## 1. Deliverable verification

Every Agent verifies the latest saved version of each Deliverable it creates or modifies.
Verification of a Working Document does not replace verification of separate Deliverables.

1. Final Minutes and other Deliverables require full Content, Writing and Formatting verification.
2. Meeting Working Records require accurate, verified persistence only.
3. Verify the three dimensions separately:
   1. **Content Quality.** Completeness, correctness, approved Scope and source fidelity.
   2. **Writing Compliance.** The [Global Writing Rules](../../rules/global-writing-rules.md) and the correct Writing Mode.
   3. **Formatting Compliance.** The artifact format and the applicable Operating Guide.
4. Apply output-specific checks that the assigned role and Deliverable require.
5. Apply the language rules in the [Global Communication Rules](../../rules/global-communication-rules.md).

## 2. Self-check steps

Every Lifecycle points to these steps. A change to quality checking changes only this Skill.
For every artifact that requires full verification, perform these steps in order:

1. Read back the complete saved artifact. A draft in the Conversation is not evidence.
2. **Content.** Check each Local QA criterion in the artifact's Operating Guide.
3. **Writing.** Check each rule of the artifact's Writing Mode. In Strict Mode, check every sentence.
4. **Formatting.** Check each heading style against the Operating Guide. Check that the artifact is easy to read under Section 3.
5. Correct every failure. Read back the saved artifact again.
6. Record PASS or FAIL for each dimension with the findings.
   Record PASS only for a check you actually performed.

## 3. Formatting checkpoints

1. Verify Formatting after creating and saving Job Records and Final Minutes.
2. Verify final Formatting again at Protocol completion.
3. Routine edits need not each trigger a full Formatting check.

Formatting must provide readable hierarchy, natural information flow, visual balance and quick navigation.
It must help readers follow, understand and scan the artifact.
Apply the rules for the artifact format: Google Docs, Markdown or another format.

## 4. Operating Guides

1. A Document Operating Guide owns its document's Purpose, Names, Metadata, Sections, Formatting and Local QA criteria.
2. Lifecycle actions and cross-resource execution belong in the Plugin Skills.
3. Apply structural refinements prospectively. Preserve historical records and approved formats.

## 5. Independent QA Workflow

Flow, part 1: user requests a QA Job → Execution Agent confirms the QA Scope.
Flow, part 2: inspection, usually by a Sub-agent → QA report → Completion Notice.

1. The user requests a QA Job from the Execution Agent through a Meeting or directly.
2. The Execution Agent runs it as a Job Scope under the [execution-agent](../execution-agent/SKILL.md) Lifecycle, usually through a Sub-agent.
3. A QA Job may be review-only. It may run periodically.
4. Assessments and reports must be independent, complete and objective.
5. Inspect every approved item at the authorized depth.
6. Inspect other working Scopes only within specifically approved Job Scope.
7. Writing Compliance is compulsory for documents subject to full QA.

Possible dimensions include structure, Operating Guide compliance, requirement fidelity, Decision-to-Deliverable Fidelity and Context authority.

## 6. Fidelity inspection

1. Compare full substantive meaning: intent, requirements, constraints, qualifications and approved revisions.
2. Identify omissions, weakening, excessive editing, unauthorized additions and changed requirements.
3. Trace the earliest verified divergence and its downstream effect.
4. Source citations alone do not establish fidelity.

## 7. QA reporting

Each inspected item needs:

- Exact source and target references.
- Criteria.
- Evidence.
- Findings.
- A result: PASS, FAIL or Unable to Verify.

1. Fidelity findings identify a useful correction starting point and final impact.
2. Report inadequate evidence without presuming compliance.

## 8. Limits

1. Complete every approved audit item without cached PASS reuse or automatic skipping.
2. A review-only QA Job does not edit inspected resources.
3. QA reports identify deficiencies but do not authorize correction.
4. A completed audit may contain failed or unverifiable findings.
