# Customer Churn Analysis — Portfolio Project

**Role:** Data Analysis Capstone  
**Tools:** Python, Pandas, SciPy, Scikit-learn, Matplotlib, Seaborn  
**Dataset:** 500 customer records

## Business question
Which customer segments show higher churn, and what retention actions should the business test?

## Result snapshot
- Overall churn: 10.6%
- Month-to-month churn: 20.6%
- One-year contract churn: 4.3%
- Logistic regression baseline ROC-AUC: 0.987 (holdout split; exploratory only)

## Recommendation
Prioritize first-year onboarding, test optional contract incentives with a randomized control group, and investigate payment friction. Validate impact using 90- and 180-day retention.

## Evidence
See `reports/executive_summary.pdf`, `reports/technical_report.pdf`, `presentation/business_presentation.pptx`, notebooks and the visualizations folder.

## Caveat
The dataset has 500 rows and limited context. Results are not causal and should be validated on representative, time-stamped production data before business deployment.
