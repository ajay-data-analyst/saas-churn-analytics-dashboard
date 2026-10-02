# Assumptions and Limitations

## Dataset
The IBM Telco Customer Churn dataset is reframed here as a SaaS subscription analytics model.

## Snapshot
The source is treated as a customer/subscription snapshot, not a complete event stream.

## Cohort
Cohort analysis uses available customer/start-cohort information and does not represent longitudinal customer survival tracking.

## NRR
`Cohort MRR Momentum` is used instead of true Net Revenue Retention because the available data does not provide complete historical revenue movement.

## LTV
`Avg Realized Revenue per Customer` and `Avg Realized Revenue - Churned` are realized-revenue measures, not predictive Customer Lifetime Value models.

## Time Intelligence
Time-intelligence calculations based on Subscription Start Date represent the available start-cohort/new-business basis, not a complete historical MRR ledger.

## Business Impact
No client deployment, client revenue impact, or quantified business outcome is claimed.

## Data Quality
Conclusions are limited to the fields and transformations available in the source dataset and model.
