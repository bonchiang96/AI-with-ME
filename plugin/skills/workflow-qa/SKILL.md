---
name: workflow-qa
description: The AI with ME Deliverable quality rules and the Independent QA Workflow. Holds the writing checking and save checks every Lifecycle runs on Final Minutes, Knowledge Bases, Job Records and Deliverables. Defines how an Execution Agent runs an independent, complete and objective QA Job with PASS, FAIL or Unable to Verify results. Use when verifying any Deliverable or when the user requests a QA Job.
compatibility: Requires the Google Drive and Google Docs connectors through the host. The Plugin does not ship the connectors.
---

# Quality and Independent QA

## 1. Deliverable verification

Every Agent verifies the latest saved version of each Deliverable it creates or modifies.
Verification of a Working Document does not replace verification of separate Deliverables.

1. Final Minutes and other Deliverables require full Content, Writing and Formatting verification.
2. Meeting Records require accurate, verified persistence only.
3. Verify the three dimensions separately:
   1. **Content Quality.** Completeness, correctness, approved Scope and source fidelity.
      Information the user provides is certified by the user. Never mark it FAIL, unverified or Unable to Verify for lack of third-party sources.
   2. **Writing Compliance.** Use the [global-writing-rules](../global-writing-rules/SKILL.md) Skill with the correct Writing Mode.
   3. **Formatting Compliance.** The artifact format and the applicable Operating Guide.
4. Apply output-specific checks that the assigned role and Deliverable require.
5. Use the language rules in the [global-communication-rules](../global-communication-rules/SKILL.md) Skill.

## 2. Self-check steps

Every Lifecycle points to these steps. A change to quality checking changes only this Skill.

### 2.1 Writing checking

1. Writing checking applies to Final Minutes, Knowledge Bases and text Deliverables.
   It follows the checking rules in the [global-writing-rules](../global-writing-rules/SKILL.md) Skill Section 8.
2. Other outputs follow the Global Writing Rules without separate checking.
   Examples are Meeting Records, Job Records, Deliverable Guidelines, Identity Context and inbox messages.
3. Run the checking on the complete final version before it is written to Google.
   In Workspace mode, run it on the workspace version before the sync.
4. For Final Minutes and Knowledge Bases, the Parent writes and a new reviewer Sub-agent checks:
   1. The Parent gives the reviewer only the final version, its Writing Mode and the Global Writing Rules.
   2. The reviewer checks and enhances the text. It replies with feedback. It never translates the content.
   3. The Parent applies each feedback item about the Global Writing Rules.
   4. The Parent ignores feedback that changes the meaning. The Parent makes the final judgment.
   5. One reviewer round is enough.
5. Without a genuine Sub-agent, the Parent does the checking itself, with the mechanical scan.
6. Text Deliverables follow the author and reviewer roles in the [execution-agent](../execution-agent/SKILL.md) Skill Section 10.
   Text Deliverables also follow the review rounds of their Workflow.
7. Non-text Deliverables, such as a website, are outside writing checking.
   Their QA follows their Workflow and output-specific checks.
8. Writing checking includes a language check under the [global-communication-rules](../global-communication-rules/SKILL.md) Skill Section 2:
   1. The content keeps its original language, or the content language that an instruction sets under Section 2.4 of that Skill.
   2. In Final Minutes, each material Decision keeps its User's words.
      In Knowledge Bases, User's words stay with the knowledge they explain.
   3. User's words stay untranslated.

### 2.2 Save checks

For every artifact that requires full verification, perform these steps in order after it is saved:

1. Read back the complete saved artifact. A draft in the Conversation is not evidence.
2. **Content.** Check each Local QA criterion in the artifact's Operating Guide.
3. **Writing.** Confirm that writing checking under Section 2.1 ran and that the saved text matches the checked version.
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
