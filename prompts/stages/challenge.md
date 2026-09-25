# Independent challenge and exceptions

## Decision context
Does the specific bond offer acceptable credit and relative value, separately from the integrity of its label, KPI and contractual incentives?

## Assignment
Challenge the strongest conclusion with contrary evidence, alternative causal explanations, missing data, model assumptions and double counting. Classify unresolved issues MINOR, MATERIAL or CRITICAL and record remediation. Independence is a human/host process requirement, not authenticated by this engine. Never hide an issue merely to reach approval.

## Required output sections
- `source_challenge`: substantive analysis linked to claim IDs.
- `model_and_method_limits`: substantive analysis linked to claim IDs.
- `material_issues`: substantive analysis linked to claim IDs.

## Evidence and methodology
Use the mandate and registered primary evidence with edition, applicability, date and limitations. Source references are in `references/standards.json` from the repository root.

## Return contract
Return the structured artifact in `schemas/artifact.schema.json`; copy run_id, input_digest, stage_id and revision from the current packet. Never recycle IDs from a demo. Source uncertainty is not resolved by lowering confidence alone: preserve a gap or issue.

## Domain boundary
A focused companion to the existing Sustainable Bond Diligence Agent, reusing its original bond helpers. An SLB is not assumed to earmark proceeds. Coupon step-up PV is conditional, not a probability-weighted value or incentive-sufficiency verdict.
