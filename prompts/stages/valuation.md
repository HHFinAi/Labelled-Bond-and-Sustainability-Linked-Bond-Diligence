# Contract economics and relative value

## Decision context
Does the specific bond offer acceptable credit and relative value, separately from the integrity of its label, KPI and contractual incentives?

## Assignment
Price a regular option-free coupon-date illustration only when assumptions fit. Real-world accrued interest, day count, settlement, curves and options need a specialist model. Calculate step-up value conditional on trigger; disclose call-before-test risks and period indexing. Match currency, duration, rank, issuer and liquidity for greenium comparison.

## Required output sections
- `cashflow_schedule`: substantive analysis linked to claim IDs.
- `conditional_stepup`: substantive analysis linked to claim IDs.
- `greenium_comparability`: substantive analysis linked to claim IDs.
- `credit_vs_label_conclusions`: substantive analysis linked to claim IDs.

## Evidence and methodology
Use ICMA-SLBP with edition, applicability, date and limitations. Source references are in `references/standards.json` from the repository root.

## Return contract
Return the structured artifact in `schemas/artifact.schema.json`; copy run_id, input_digest, stage_id and revision from the current packet. Never recycle IDs from a demo. Source uncertainty is not resolved by lowering confidence alone: preserve a gap or issue.

## Domain boundary
A focused companion to the existing Sustainable Bond Diligence Agent, reusing its original bond helpers. An SLB is not assumed to earmark proceeds. Coupon step-up PV is conditional, not a probability-weighted value or incentive-sufficiency verdict.

A domain calculation must pass recomputation. The minimal runnable illustration is `slb_stepup_pv`; other needed specialist models must remain explicitly external and independently reviewed.
