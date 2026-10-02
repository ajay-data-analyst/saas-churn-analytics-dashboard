# Data Model

## Purpose
The model supports SaaS subscription churn, retention, revenue, tenure, cohort, customer-risk, and feature-adoption analysis.

## Core Tables
- `Fact_Subscriptions`
- `Dim_Customers`
- `Dim_Date`
- `_Measures`

## Modeling Approach
The model follows a star-schema-oriented structure with subscription/customer facts supported by customer and date dimensions.

## Date Table
`Dim_Date` covers 2018-01-01 through 2024-12-31 with 2,557 continuous dates. The `Date` column is configured as the model date table.

## Relationships
The validated project retains the original two model relationships. No unsupported Tenure Bucket Sort relationship was added.

## Derived Concepts
- Churn Flag
- Tenure Bucket
- Tenure Bucket Sort
- Feature Adoption Count
- Subscription Start Date
- Revenue and MRR measures
- Retention and cohort measures

## Snapshot Limitation
The dataset represents customer-level subscription information at a snapshot rather than a complete event-level subscription history. Time-intelligence calculations using Subscription Start Date therefore describe the available start-cohort/new-business basis, not a full historical MRR ledger.

## Validation
The documented PBIR validation completed with 152 files and 0 errors.
