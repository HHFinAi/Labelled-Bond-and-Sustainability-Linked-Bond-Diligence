# Investment committee and accountable review

## Decision context
Does the specific bond offer acceptable credit and relative value, separately from the integrity of its label, KPI and contractual incentives?

## Assignment
Integrate findings without changing their qualification. Separate facts, inferences, assumptions and calculations; cite evidence IDs and dates. Preserve unknown conclusions. Complete the domain-assessment declarations, register unresolved material issues, and submit for human research review. Do not certify legal compliance or investment performance.

## Required output sections
- `investment_question_and_answer`: substantive analysis linked to claim IDs.
- `financial_vs_sustainability_conclusions`: substantive analysis linked to claim IDs.
- `evidence_and_calculations`: substantive analysis linked to claim IDs.
- `decision_conditions_and_limits`: substantive analysis linked to claim IDs.

## Evidence and methodology
Use the mandate and registered primary evidence with edition, applicability, date and limitations. Source references are in `references/standards.json` from the repository root.

## Return contract
Return the structured artifact in `schemas/artifact.schema.json`; copy run_id, input_digest, stage_id and revision from the current packet. Never recycle IDs from a demo. Source uncertainty is not resolved by lowering confidence alone: preserve a gap or issue.

## Domain boundary
A focused companion to the existing Sustainable Bond Diligence Agent, reusing its original bond helpers. An SLB is not assumed to earmark proceeds. Coupon step-up PV is conditional, not a probability-weighted value or incentive-sufficiency verdict.

Required typed domain-assessment fields (declarations, not automated truth verification):
```json
{
  "credit_conclusion": [
    "acceptable_for_review",
    "unacceptable",
    "not_established"
  ],
  "label_conclusion": [
    "supported",
    "unsupported",
    "not_established"
  ],
  "impact_conclusion": [
    "evidenced",
    "claimed_only",
    "not_established"
  ],
  "stepup_basis": [
    "conditional_not_expected",
    "not_applicable"
  ],
  "credit_label_conclusions_separate": [
    true
  ]
}
```
