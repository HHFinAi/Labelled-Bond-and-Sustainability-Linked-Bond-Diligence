---
name: bond-credit
description: Underlying credit assessment for institutional sustainable-finance research; return evidence-linked findings, assumptions, gaps and reviewable outputs.
license: MIT
metadata:
  author: HHFinAi
  version: "0.2.0"
---
# Underlying credit assessment

Read `../../AGENTS.md` and `../../prompts/stages/credit.md` relative to this skill directory. Obtain the current stage packet using the repository CLI. Do not create or claim unavailable source access.

## Task
Assess cash generation, leverage, interest cover, maturity schedule, covenants, refinancing, seniority and recovery. Green/social labels do not waive credit work. Separate rates, credit spread, optionality, liquidity and currency risks.

## Deliverable
Return the fields in `../../schemas/artifact.schema.json`; use the current run ID and input digest. Required sections: repayment_capacity, refinancing_and_liquidity, downside_recovery, peer_comparability. Include source IDs, scope, periods, methods and material gaps. Call only allowlisted calculations with explicit provenance; missing evidence means NEEDS_DATA, not invented values.

## Limit
A focused companion to the existing Sustainable Bond Diligence Agent, reusing its original bond helpers. An SLB is not assumed to earmark proceeds. Coupon step-up PV is conditional, not a probability-weighted value or incentive-sufficiency verdict.
