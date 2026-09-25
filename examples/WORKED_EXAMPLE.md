# Worked example — Labelled-Bond and Sustainability-Linked-Bond Diligence Agent

**SYNTHETIC / RESEARCH_ONLY. All company, portfolio, instrument and outcome values are fictional. No capital should be deployed from this example.**

## Investment-relevant observation
The fictional bond pays an additional annual 25 basis points on a face amount of 100, divided into semiannual payments, in periods 7–10 inclusive. The function discounts each extra 0.125 payment at a nominal annual 5% rate with two coupon periods. The result is conditional on trigger activation.

## Reproduce the arithmetic
From the repository root:
```bash
python -m sf_agent calc --operation slb_stepup_pv --arguments examples/calculation-arguments.json
```

### Inputs
```json
{
  "face": 100,
  "step_up_bps": 25,
  "first_payment_period": 7,
  "last_payment_period": 10,
  "annual_discount": 0.05,
  "frequency": 2
}
```

### Recomputed result
```json
0.40549232117388867
```

## What the result does not establish
Do not multiply by an invented trigger probability. Confirm real observation dates, verification, notice, fallbacks and call provisions. Accrued interest, irregular periods, default and optionality need a fuller pricing model. Credit quality and label integrity remain separate.

## Diligence handoff
Fictional SLB: the coupon penalty is valued conditional on activation, while credit quality and sustainability integrity receive separate judgments.

Register source-backed inputs, contrary evidence, material data gaps and the investment constraints before replacing this illustrative result with actual research. Unit, boundary, timing, attribution and legal judgments are not supplied by arithmetic alone. No human research approval is recorded for this example.
