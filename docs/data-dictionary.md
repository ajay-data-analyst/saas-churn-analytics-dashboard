# Data Dictionary

## Fact_Subscriptions

| Field | Purpose |
|---|---|
| Customer ID | Customer identifier |
| Subscription Start Date | Derived subscription start date |
| Tenure Months | Customer tenure |
| Tenure Bucket | Tenure category |
| Tenure Bucket Sort | Sort support for tenure categories |
| Plan Type | Subscription plan |
| Payment Method | Payment method |
| Total Revenue | Realized customer revenue |
| Churn Flag | Numeric churn indicator |
| Feature Adoption Count | Count of adopted features |

## Dim_Customers
Customer-level descriptive attributes used for segmentation and filtering.

## Dim_Date

| Field | Purpose |
|---|---|
| Date | Calendar date |
| Year | Calendar year |
| Month Number | Numeric month ordering |
| Month-Year | Display month/year |
| Month Sort | Chronological ordering |

The date table covers 2018-01-01 through 2024-12-31.

## Measures
Measures are stored in `_Measures`.

Important current names:
- Retention Rate by Tenure Segment
- Cohort MRR Momentum
- Avg Realized Revenue per Customer
- Avg Realized Revenue - Churned
- Avg Tenure Months
- Avg Tenure Months - Churned

## Transformation Notes
Power Query/M creates or transforms fields including subscription start date, churn flag, tenure bucket, and feature adoption count.
