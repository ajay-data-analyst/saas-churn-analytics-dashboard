# DAX Measures

## Main Measure Groups

### Revenue and Subscription Health
- Total MRR
- ARR
- ARPU
- Revenue Churn Rate
- MRR Previous Month
- MRR SPLY
- MRR YTD
- Rolling 12M MRR
- Running Total MRR

### Churn and Retention
- Churn Rate (Logo)
- Churn Rate Previous Month
- Churn Rate Change MoM
- Retention Rate by Tenure Segment
- Cohort Churn Rate Change MoM
- Cohort MRR Momentum

### Customer Tenure and Value
- Avg Tenure Months
- Avg Tenure Months - Churned
- Avg Realized Revenue per Customer
- Avg Realized Revenue - Churned
- ARPU

### Customer Risk
Risk calculations support segmentation using churn status, plan characteristics, tenure, and feature adoption.

## DAX Techniques
The project uses CALCULATE, DATEADD, SAMEPERIODLASTYEAR, DATESINPERIOD, VAR, SWITCH, filtering, and conditional calculations.

## Important Definitions

### Retention Rate by Tenure Segment
Share of customers retained within the available tenure-segment context. It is not longitudinal customer survival.

### Cohort MRR Momentum
Start-cohort MRR comparison. It is not presented as true Net Revenue Retention.

### Avg Realized Revenue per Customer
Average `Fact_Subscriptions[Total Revenue]` within the current filter context. It is not predictive Customer Lifetime Value.

### Avg Realized Revenue - Churned
Average realized revenue for the churned population.

### Avg Tenure Months
Average customer tenure in months within the current filter context.

## Naming Principle
Measure names were revised to avoid overstating what the snapshot data can support.
