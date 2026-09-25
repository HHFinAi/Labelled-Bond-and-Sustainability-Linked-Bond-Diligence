---
name: bond-label
description: Label or KPI/SPT integrity for institutional sustainable-finance research; return evidence-linked findings, assumptions, gaps and reviewable outputs.
license: MIT
metadata:
  author: HHFinAi
  version: "0.2.0"
---
# Label or KPI/SPT integrity

Read `../../AGENTS.md` and `../../prompts/stages/label.md` relative to this skill directory. Obtain the current stage packet using the repository CLI. Do not create or claim unavailable source access.

## Task
For use-of-proceeds bonds test project selection, allocation, refinancing share, temporary management of proceeds and impact evidence. For SLBs test material KPI coverage, baseline, recalculation, peer ambition, observation date, external verification, late reporting and fallback clauses. Keep hybrid obligations separate. For the transition-bond route, assess the issuer transition strategy, material emissions coverage, science-based pathway assumptions, funded implementation, project selection and carbon-lock-in risk against the applicable dated ICMA transition guidance. Do not call a high-emitting activity aligned merely because it improves on its own past performance.

## Deliverable
Return the fields in `../../schemas/artifact.schema.json`; use the current run ID and input digest. Required sections: route_classification, proceeds_or_kpi, baseline_ambition, verification_and_fallbacks. Include source IDs, scope, periods, methods and material gaps. Call only allowlisted calculations with explicit provenance; missing evidence means NEEDS_DATA, not invented values.

## Limit
A focused companion to the existing Sustainable Bond Diligence Agent, reusing its original bond helpers. An SLB is not assumed to earmark proceeds. Coupon step-up PV is conditional, not a probability-weighted value or incentive-sufficiency verdict.
