# Operating Principles

Apply these principles throughout AI with ME operation.

## 1. Framework definition

1. **Framework identity.** The name “AI with ME - Operating Framework” covers:

   - The Plugin.
   - Google governance resources.
   - Their operating relationships.

   It is a portable AI Operating Framework across supported environments.

2. **Core purpose.** The Framework's core purpose is knowledge transfer.
   AI helps users express their knowledge accurately in written form.
   Other AI Agents and people must be able to read and understand that knowledge.

   Support reusable, portable work with:

   - Clear responsibility.
   - Bounded Scope.
   - User decisions.
   - Durable authoritative records.

   It should reduce unnecessary source reads and duplicated instructions.

3. **Meaning of requirements.** Interpret these requirement terms consistently:

   1. “Must” states a required outcome.
   2. “Should” preserves an intended preference.
   3. “May” identifies permitted flexibility.

   Conditions and qualifications remain part of each requirement.

4. **Substantive authority.** The user remains the final decision-maker. Confirmed governing decisions establish substantive requirements.

   The following do not independently authorize execution:

   - Messages.
   - Proposals.
   - Accepted Findings.
   - Advisory Experiences.

5. **Interaction modes.** Agents choose interaction modes under [Global Communication Rules Section 5](../../../rules/global-communication-rules.md#5-interaction-modes).

## 2. Binding Non-functional Requirements

These Non-functional Requirements bind relevant design and maintenance of:

- Requirements.
- The AI Plugin.
- Agent Instructions.
- Lifecycles.
- Workflows.

1. **AI Management.** The Framework governs AI Management. Keep it distinct from Software Management, whose design principles and expectations differ.

2. **AI autonomy.** The Framework defines:

   - Source authority.
   - Agent responsibilities.
   - Scope.
   - Dependencies.
   - Forward Lifecycles.
   - Workflows.
   - Required approvals.
   - Expected outcomes.

   The executing AI selects practical methods within these requirements and its available capabilities. It solves operational problems using its own judgment.

   Agent Lifecycles must preserve:

   - Essential stages.
   - Decisions.
   - Information handling.
   - Handoffs.

3. **Priorities and boundaries.** Define meaningful priorities and essential Scope boundaries.
   Settle forward-flow requirements under [Section 2.8](#2-binding-non-functional-requirements).
   Allow reasonable ambiguity in implementation methods without leaving incompatible forward flows unresolved.

   Do not specify every possible:

   - Edge case.
   - Condition.
   - Micro-boundary.

4. **Failure Handling.** AI must use its judgment when execution encounters difficulties. It must act within authorized Scope and record actual outcomes. Report necessary assistance.

   Do not predesign Failure Handling methods for the AI.

   Normal AI execution must not require:

   - Fixed retry counts.
   - Exhaustive recovery branches.

   Delegated acceptance review follows [Execution Lifecycle Section 4](../../execution-agent/references/lifecycle.md#4-execution-parent-and-sub-agents).

5. **AI behavior verification.** Individual AI behavior and choices may vary between executions.

   Do not require:

   - Deterministic, repeatable verification of individual AI behavior.
   - A universal AI-response Verification stage.

   Actual Deliverable QA follows [Quality Section 1](../../workflow-qa/references/quality.md#1-deliverable-quality-and-independent-qa).

6. **Writing, design and operating preferences.** Preserve the following as binding Non-functional Requirements:

   - AI-native constraints.
   - Writing and design principles.
   - Relevant user operating preferences.

   Apply [Global Writing Rules](../../../rules/global-writing-rules.md) and [Global Communication Rules](../../../rules/global-communication-rules.md).

7. **Requirement numbering.** Use the file and its Section numbering to locate requirements. Do not add parallel R-prefixed identifiers to every requirement.

8. **Forward-flow completeness.** Requirements must settle every item that determines:

   - Step order.
   - The responsible owner.
   - The approver.
   - Resources read.
   - Resources written.
   - The outcome.

   An item belongs in Requirements when two developers could otherwise implement incompatible flows.
   Implementation design may remain deferred only when the required outcome is stated.
   Detailed design boundaries follow [Environments and Deferred Work Section 2.5](environments.md#2-baseline-acceptance-and-deferred-development).

9. **Requirements inspection.** After all modifications, independently inspect the complete Requirements artifact.
   Cover the three quality dimensions in [Quality Section 1.2](../../workflow-qa/references/quality.md#1-deliverable-quality-and-independent-qa).

9. **Consolidated maintenance.** Maintain every file by consolidation rather than appending.
   Working Records and Job Records keep their chronological history.
   Every other file holds only current truth, kept light and accurate.
