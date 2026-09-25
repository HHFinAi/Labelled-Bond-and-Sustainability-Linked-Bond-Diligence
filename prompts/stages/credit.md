# Underlying credit assessment

## Decision context
Does the specific bond offer acceptable credit and relative value, separately from the integrity of its label, KPI and contractual incentives?

## Assignment
Assess cash generation, leverage, interest cover, maturity schedule, covenants, refinancing, seniority and recovery. Green/social labels do not waive credit work. Separate rates, credit spread, optionality, liquidity and currency risks.

## Required output sections
- `repayment_capacity`: substantive analysis linked to claim IDs.
- `refinancing_and_liquidity`: substantive analysis linked to claim IDs.
- `downside_recovery`: substantive analysis linked to claim IDs.
- `peer_comparability`: substantive analysis linked to claim IDs.

## Evidence and methodology
Use the mandate and registered primary evidence with edition, applicability, date and limitations. Source references are in `references/standards.json` from the repository root.

## Return contract
Return the structured artifact in `schemas/artifact.schema.json`; copy run_id, input_digest, stage_id and revision from the current packet. Never recycle IDs from a demo. Source uncertainty is not resolved by lowering confidence alone: preserve a gap or issue.

## Domain boundary
A focused companion to the existing Sustainable Bond Diligence Agent, reusing its original bond helpers. An SLB is not assumed to earmark proceeds. Coupon step-up PV is conditional, not a probability-weighted value or incentive-sufficiency verdict.
