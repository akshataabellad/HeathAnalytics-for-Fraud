# Healthcare Insurance Fraud & Anomaly Intelligence

## Overview

This project explores healthcare insurance claims to identify provider patterns that may warrant further review. It combines data preparation, exploratory analysis, machine learning, SQL analysis, and a Power BI dashboard to make potential anomalies easier to investigate.

A model flag is an indicator for review, not proof of fraud. Any real-world decision would require qualified human investigation and appropriate privacy safeguards.

## Project goals

- Prepare and explore healthcare claims and provider data.
- Look for unusual claim and reimbursement patterns.
- Build provider-level features for analysis.
- Compare supervised classification with unsupervised anomaly detection.
- Summarize findings with SQL and an interactive Power BI report.

## Tools and methods

| Tool or method | Role in the project |
|---|---|
| Python, Pandas, NumPy | Data preparation and analysis |
| Matplotlib, Seaborn | Exploratory visualizations |
| scikit-learn Random Forest | Supervised provider classification |
| scikit-learn Isolation Forest | Unsupervised anomaly detection |
| MySQL | Provider-level storage and SQL analysis |
| Power BI | Interactive reporting |
| Jupyter Notebook | Analysis and experimentation |

## Workflow

1. Load claims, beneficiary, inpatient, and outpatient data.
2. Inspect and clean the data, including missing values and duplicates.
3. Explore claim and provider patterns.
4. Build provider-level features from relevant claim information.
5. Train and evaluate a Random Forest classifier and use Isolation Forest to surface unusual observations.
6. Store or query analysis results with MySQL.
7. Present selected findings in a Power BI dashboard.

## Dashboard

The project discussion describes a dashboard with provider counts, potentially fraudulent provider counts, fraud rate, fraud distribution, average reimbursement by fraud status, high-risk providers, and inpatient versus outpatient claim analysis. Add a dashboard screenshot here only after confirming that it contains no sensitive information.

## Reported model results

The project notes report the following Random Forest evaluation results:

| Metric | Reported result |
|---|---:|
| Accuracy | 92.14% |
| Precision | 55.97% |
| Recall | 74.26% |
| F1-score | 63.83% |

These figures are included as previously reported project results and have not been independently reproduced from files in this repository. Before relying on or presenting them, verify the evaluation code, data split, target definition, and class balance. Accuracy alone can be misleading when fraud cases are uncommon; precision and recall should be considered in context.

## Data privacy

Do not commit raw beneficiary or patient records, personally identifying information, protected health information, credentials, or private database exports. Use only data that you are authorized to share, and check the dataset and repository policies before publishing. Prefer a small, clearly documented synthetic or approved sample if an example dataset is needed.

## Reproducibility

The project files and exact run instructions were not available when this README was prepared. Add the verified notebook or script names, dependency installation steps, database setup, and dashboard access instructions after confirming the actual files. Do not publish private datasets or credentials as part of those instructions.

## Limitations

- A model can reflect gaps or bias in its training data and may miss fraud or flag legitimate behavior.
- Performance depends on the data, labels, feature choices, and evaluation design.
- An anomaly is not necessarily fraud; predictions should support investigation, not replace it.

## Future improvements

- Document reproducible setup and evaluation steps.
- Validate performance on an appropriately held-out dataset and report class balance.
- Add explainability and calibration checks.
- Improve privacy controls and data governance documentation.

## Author

Developed as a data analytics and machine learning project.
