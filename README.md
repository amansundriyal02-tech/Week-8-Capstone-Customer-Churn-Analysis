# Week 8 Capstone: Customer Churn Business Analysis

## Executive overview
This capstone investigates customer churn using a supplied dataset of **500 customers**. The business objective is to identify high-risk segments and propose measurable retention actions.

## Business problem
Customer churn reduces recurring revenue and increases replacement-acquisition costs. The analysis examines how churn varies by contract type, tenure and payment method, then builds an exploratory classification baseline.

## Key findings
- Overall churn: **10.6%** (53 of 500); 95% Wilson confidence interval: **8.2%–13.6%**.
- Month-to-month churn: **20.6%**; one-year: **4.3%**; two-year: **6.9%**.
- Churn is concentrated in the first 12 months in this sample. Observed 0% churn in tenure groups above 12 months should be validated against a larger, time-based dataset.
- Contract type is associated with churn (chi-square p=9.59e-07).

## Recommendations
1. Launch a structured first-year onboarding and engagement program.
2. Pilot transparent, optional longer-contract incentives for month-to-month customers.
3. Investigate payment friction and capture customer-stated churn reasons.
4. Run a controlled pilot; monitor 90/180-day retention, complaints, conversion and offer cost.
5. Do not operationalize the predictive model until it is validated on newer unseen data.

## Repository structure
- `data/raw/` original uploaded data
- `data/processed/` cleaned analysis dataset
- `notebooks/` cleaning, EDA and statistical/model analysis
- `reports/` executive and technical reports
- `presentation/` business presentation
- `visualizations/` seven exported charts
- `src/` reproducible Python pipeline
- `capstone_analysis.ipynb` consolidated portfolio notebook

## Reproduce
```bash
python -m pip install -r requirements.txt
python src/run_analysis.py
```
Open notebooks from the repository root in Jupyter.

## Data quality and limitations
The raw dataset contains 500 rows and no missing values or duplicate rows; cleaned output preserves all 500. The data dictionary and time coverage were not supplied. No churn reasons, support interactions, acquisition channel, timestamps or marketing spend are available. The dataset appears small and may be synthetic; treat results as directional, not representative of a real customer base. Statistical association is not causation. Model scores require external and time-based validation.

## Portfolio summary
**Problem:** Where is churn concentrated?
**Method:** EDA, segment rates, confidence interval, chi-square tests, Welch t-test, logistic regression.
**Outcome:** actionable first-year and month-to-month retention pilot recommendations.
