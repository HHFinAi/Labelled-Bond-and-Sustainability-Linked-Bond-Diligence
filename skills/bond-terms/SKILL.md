---
name: bond-terms
description: Instrument and creditor rights for institutional sustainable-finance research; return evidence-linked findings, assumptions, gaps and reviewable outputs.
license: MIT
metadata:
  author: HHFinAi
  version: "0.2.0"
---
# Instrument and creditor rights

Read `../../AGENTS.md` and `../../prompts/stages/terms.md` relative to this skill directory. Obtain the current stage packet using the repository CLI. Do not create or claim unavailable source access.

## Task
Identify ISIN or contract ID, legal obligor, guarantor, rank, currency, security, call rights, observation dates and governing documents. Do not transfer parent metrics to the wrong obligor. Obtain counsel review for enforcement or contested clauses.

## Deliverable
Return the fields in `../../schemas/artifact.schema.json`; use the current run ID and input digest. Required sections: obligor_guarantor, rank_recourse_covenants, coupon_call_maturity, documentation_gaps. Include source IDs, scope, periods, methods and material gaps. Call only allowlisted calculations with explicit provenance; missing evidence means NEEDS_DATA, not invented values.

## Limit
A focused companion to the existing Sustainable Bond Diligence Agent, reusing its original bond helpers. An SLB is not assumed to earmark proceeds. Coupon step-up PV is conditional, not a probability-weighted value or incentive-sufficiency verdict.
