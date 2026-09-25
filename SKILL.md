---
name: labelled-bond-slb-diligence-agent
description: Does the specific bond offer acceptable credit and relative value, separately from the integrity of its label, KPI and contractual incentives? Institutional buy-side research workflow with auditable evidence, calculations and human review; no autonomous trading.
license: MIT
metadata:
  author: HHFinAi
  version: "0.2.0"
---
# Labelled-Bond and Sustainability-Linked-Bond Diligence Agent

Use for labelled bonds and slbs under a specified investment mandate. Read `AGENTS.md`, then select a route from `agent.json`. Follow `WORKFLOW.md` and the CLI research loop. Copy the entire repository, not just this file: scripts, prompts, schemas and references are required.

A compatible filesystem-enabled agent host may discover this skill; activation has not been certified for specific products. Text-only use applies the methodology manually and does not enforce the Python controls.

A focused companion to the existing Sustainable Bond Diligence Agent, reusing its original bond helpers. An SLB is not assumed to earmark proceeds. Coupon step-up PV is conditional, not a probability-weighted value or incentive-sufficiency verdict.

Do not run a synthetic fixture as live research. Start with `examples/research-request-template.json`, replace every placeholder and register permitted evidence. Inspect `docs/INSTITUTIONAL_QUALITY.md` and `docs/AUDIT.md` before relying on outputs.
