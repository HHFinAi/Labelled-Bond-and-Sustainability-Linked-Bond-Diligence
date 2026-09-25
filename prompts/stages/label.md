# Label or KPI/SPT integrity

## Decision context
Does the specific bond offer acceptable credit and relative value, separately from the integrity of its label, KPI and contractual incentives?

## Assignment
For use-of-proceeds bonds test project selection, allocation, refinancing share, temporary management of proceeds and impact evidence. For SLBs test material KPI coverage, baseline, recalculation, peer ambition, observation date, external verification, late reporting and fallback clauses. Keep hybrid obligations separate. For the transition-bond route, assess the issuer transition strategy, material emissions coverage, science-based pathway assumptions, funded implementation, project selection and carbon-lock-in risk against the applicable dated ICMA transition guidance. Do not call a high-emitting activity aligned merely because it improves on its own past performance.

## Required output sections
- `route_classification`: substantive analysis linked to claim IDs.
- `proceeds_or_kpi`: substantive analysis linked to claim IDs.
- `baseline_ambition`: substantive analysis linked to claim IDs.
- `verification_and_fallbacks`: substantive analysis linked to claim IDs.

## Evidence and methodology
Use ICMA-SLBP, ICMA-GBP, ICMA-CTBG with edition, applicability, date and limitations. Source references are in `references/standards.json` from the repository root.

## Return contract
Return the structured artifact in `schemas/artifact.schema.json`; copy run_id, input_digest, stage_id and revision from the current packet. Never recycle IDs from a demo. Source uncertainty is not resolved by lowering confidence alone: preserve a gap or issue.

## Domain boundary
A focused companion to the existing Sustainable Bond Diligence Agent, reusing its original bond helpers. An SLB is not assumed to earmark proceeds. Coupon step-up PV is conditional, not a probability-weighted value or incentive-sufficiency verdict.
