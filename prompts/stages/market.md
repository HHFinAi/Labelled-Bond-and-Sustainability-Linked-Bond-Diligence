# Market context and implementation evidence

## Decision context
Does the specific bond offer acceptable credit and relative value, separately from the integrity of its label, KPI and contractual incentives?

## Assignment
For public instruments obtain a timestamped scoped quote, price convention, liquidity, currency and funding/borrow evidence where relevant. For private structures obtain reviewed contracts and eligibility. Portfolio accounting and compliance assessments may remain RESEARCH_ONLY. No invented price or automatic hedge.

## Required output sections
- `market_or_contract_evidence`: substantive analysis linked to claim IDs.
- `liquidity_funding_access`: substantive analysis linked to claim IDs.
- `portfolio_context`: substantive analysis linked to claim IDs.

## Evidence and methodology
Use the mandate and registered primary evidence with edition, applicability, date and limitations. Source references are in `references/standards.json` from the repository root.

## Return contract
Return the structured artifact in `schemas/artifact.schema.json`; copy run_id, input_digest, stage_id and revision from the current packet. Never recycle IDs from a demo. Source uncertainty is not resolved by lowering confidence alone: preserve a gap or issue.

## Domain boundary
A focused companion to the existing Sustainable Bond Diligence Agent, reusing its original bond helpers. An SLB is not assumed to earmark proceeds. Coupon step-up PV is conditional, not a probability-weighted value or incentive-sufficiency verdict.
