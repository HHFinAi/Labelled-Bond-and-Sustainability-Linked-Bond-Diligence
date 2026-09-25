# Executable operation catalogue

Every operation requires supplied assumptions/provenance. No market or issuer data are inferred.

## `allocation_coverage`
```python
allocation_coverage(eligible_allocated: 'float', net_proceeds: 'float') -> 'float'
```
See source code and domain methodology for assumptions.

Input units: `{"eligible_allocated": "$money", "net_proceeds": "$money"}`. Output unit/type: `decimal_fraction`.

## `bond_price`
```python
bond_price(face: 'float', annual_coupon: 'float', yield_to_maturity: 'float', years: 'float', frequency: 'int') -> 'float'
```
Coupon-date full price; accrued interest is zero at the assumed valuation date.

Input units: `{"face": "$money", "annual_coupon": "decimal", "yield_to_maturity": "decimal", "years": "years", "frequency": "payments_per_year"}`. Output unit/type: `$money`.

## `bond_risk`
```python
bond_risk(face: 'float', annual_coupon: 'float', yield_to_maturity: 'float', years: 'float', frequency: 'int') -> 'dict'
```
See source code and domain methodology for assumptions.

Input units: `{"face": "$money", "annual_coupon": "decimal", "yield_to_maturity": "decimal", "years": "years", "frequency": "payments_per_year"}`. Output unit/type: `bond_risk_metrics`.

## `dscr`
```python
dscr(cash_available: 'float', debt_service: 'float') -> 'float'
```
See source code and domain methodology for assumptions.

Input units: `{"cash_available": "$money", "debt_service": "$money"}`. Output unit/type: `multiple`.

## `greenium`
```python
greenium(labelled_spread_bps: 'float', matched_conventional_spread_bps: 'float') -> 'float'
```
Positive value = labelled bond's tighter spread. Comparability is external.

Input units: `{"labelled_spread_bps": "basis_points", "matched_conventional_spread_bps": "basis_points"}`. Output unit/type: `basis_points`.

## `holding_period_return`
```python
holding_period_return(initial_dirty_price: 'float', exit_dirty_price: 'float', cash_income: 'float', funding_cost: 'float', transaction_cost: 'float') -> 'float'
```
See source code and domain methodology for assumptions.

Input units: `{"initial_dirty_price": "$money", "exit_dirty_price": "$money", "cash_income": "$money", "funding_cost": "$money", "transaction_cost": "$money"}`. Output unit/type: `decimal_return`.

## `npv`
```python
npv(cashflows: 'list[float]', annual_discount: 'float') -> 'float'
```
Periodic NPV; cashflows[0] is at time zero, then annual periods.

Input units: `{"cashflows": "$money", "annual_discount": "decimal"}`. Output unit/type: `$money`.

## `scale`
```python
scale(value: 'float', factor: 'float') -> 'float'
```
Explicit arithmetic conversion; external unit semantics need human review.

Input units: `{"value": "$input_unit", "factor": "conversion_factor"}`. Output unit/type: `$output_unit`.

## `slb_stepup_pv`
```python
slb_stepup_pv(face: 'float', step_up_bps: 'float', first_payment_period: 'int', last_payment_period: 'int', annual_discount: 'float', frequency: 'int') -> 'float'
```
PV of extra coupons IF the contractual step-up triggers; not expected value.

Input units: `{"face": "$money", "step_up_bps": "basis_points", "first_payment_period": "period_index", "last_payment_period": "period_index", "annual_discount": "decimal", "frequency": "payments_per_year"}`. Output unit/type: `$money`.
