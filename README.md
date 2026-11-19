# Employee Attrition & Survival Analysis
A machine learning and survival analysis project focused on modeling employee attrition patterns, estimating time-to-event retention probabilities, and evaluating individual turnover risk across employee tenure.

## Overview
- *Dataset:* HR employee attrition / churn dataset (hr_employee_churn_data.csv)
- *Core Notebook:* HR EMPLOYEE ATTRITION.ipynb
- *Approach:* Combines classical survival statistics with machine learning survival models to capture time-dependent retention behavior and risk rankings.

## Models & Methods
- *Kaplan-Meier Estimator:* Non-parametric survival curve to visualize overall employee retention over time.
- *Cox Proportional Hazards (CoxPH):* Semi-parametric baseline survival model evaluated using concordance index (C-index).
- *Random Survival Forest (RSF):* Tree-based survival model evaluated with Mean Time-dependent AUC and Integrated Brier Score (IBS).
- *XGBoost Survival:* Gradient-boosted survival model evaluated with risk-score-based Mean Time-dependent AUC.

## Evaluation Metrics
- *Concordance Index (C-index):* Measures rank-ordering performance of predicted risk.
- *Mean Time-Dependent AUC:* Evaluates discrimination across survival time points.
- *Integrated Brier Score (IBS):* Evaluates calibration and survival probability accuracy over time for models providing survival functions (such as Random Survival Forest).
