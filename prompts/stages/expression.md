# Investment-decision handoff

## Decision context
Does the specific bond offer acceptable credit and relative value, separately from the integrity of its label, KPI and contractual incentives?

## Assignment
Connect the analytical findings to an identified instrument or portfolio decision. Separate attractive economics from mandate permission. Document price, valuation, entry conditions, downside, catalysts, liquidity, hedging and thesis breakers. PUBLIC/PRIVATE_MARKET_CANDIDATE requires every declared check to pass and reviewed quote/contract evidence; otherwise RESEARCH_ONLY or NO_INVESTMENT_ROUTE. No execution authority.

## Required output sections
- `valuation_and_entry`: substantive analysis linked to claim IDs.
- `risk_catalysts_and_thesis_breakers`: substantive analysis linked to claim IDs.
- `eligibility_review`: substantive analysis linked to claim IDs.

## Evidence and methodology
Use the mandate and registered primary evidence with edition, applicability, date and limitations. Source references are in `references/standards.json` from the repository root.

## Return contract
Return the structured artifact in `schemas/artifact.schema.json`; copy run_id, input_digest, stage_id and revision from the current packet. Never recycle IDs from a demo. Source uncertainty is not resolved by lowering confidence alone: preserve a gap or issue.

## Domain boundary
A focused companion to the existing Sustainable Bond Diligence Agent, reusing its original bond helpers. An SLB is not assumed to earmark proceeds. Coupon step-up PV is conditional, not a probability-weighted value or incentive-sufficiency verdict.
