---
name: bond-valuation
description: Contract economics and relative value for institutional sustainable-finance research; return evidence-linked findings, assumptions, gaps and reviewable outputs.
license: MIT
metadata:
  author: HHFinAi
  version: "0.2.0"
---
# Contract economics and relative value

Read `../../AGENTS.md` and `../../prompts/stages/valuation.md` relative to this skill directory. Obtain the current stage packet using the repository CLI. Do not create or claim unavailable source access.

## Task
Price a regular option-free coupon-date illustration only when assumptions fit. Real-world accrued interest, day count, settlement, curves and options need a specialist model. Calculate step-up value conditional on trigger; disclose call-before-test risks and period indexing. Match currency, duration, rank, issuer and liquidity for greenium comparison.

## Deliverable
Return the fields in `../../schemas/artifact.schema.json`; use the current run ID and input digest. Required sections: cashflow_schedule, conditional_stepup, greenium_comparability, credit_vs_label_conclusions. Include source IDs, scope, periods, methods and material gaps. Call only allowlisted calculations with explicit provenance; missing evidence means NEEDS_DATA, not invented values.

## Limit
A focused companion to the existing Sustainable Bond Diligence Agent, reusing its original bond helpers. An SLB is not assumed to earmark proceeds. Coupon step-up PV is conditional, not a probability-weighted value or incentive-sufficiency verdict.
