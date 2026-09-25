# Methodology and model boundaries

A focused companion to the existing Sustainable Bond Diligence Agent, reusing its original bond helpers. An SLB is not assumed to earmark proceeds. Coupon step-up PV is conditional, not a probability-weighted value or incentive-sufficiency verdict.

## Analytical outputs
- Credit and instrument-terms dossier
- Use-of-proceeds or KPI/SPT diligence
- Conditional step-up PV and relative-value comparison
- Separate credit, label and impact conclusions

## Calculation library
The implementation is in `sf_agent/analytics.py`; generic helpers are in `sf_agent/maths.py`. Every exposed operation has argument-unit and result-unit metadata and is callable with `python -m sf_agent calc`. Arguments are not sourced automatically. See the operation inventory below, the worked example and domain regression tests.

### Bond calculations
This module preserves the original HHFinAi v0.1.0 regular fixed-rate bond helpers. `bond_price` assumes coupon-date settlement, fixed equal coupon periods, face repayment and no options, default, accrued interest, irregular stubs or curve-based pricing. It is a flat-yield illustration, not a settlement-ready trading pricer. `bond_risk` reports modified duration, convexity and DV01 under the same assumptions.

`slb_stepup_pv` uses an annual basis-point increase divided by coupon frequency and discounts each extra coupon from the first to last payment period inclusively. Value is conditional on activation. It does not supply trigger probability, accrued interest, contractual notice timing or call behavior. `greenium` is conventional spread minus labelled spread in basis points; a positive value denotes a tighter labelled spread, not causal attribution to the label. `allocation_coverage` compares eligible allocated proceeds with net proceeds and rejects over-allocation under that scoped accounting convention. Refinancing, impact and credit quality remain separate.


## Evidence status
Causal and legal interpretations remain human judgments. The software is not a complete implementation or certification of the referenced standards. Read the exact applicable original documents; the dated source register gives the verification scope. Proposed changes and future validation dates must not be applied retrospectively or represented as current law.
