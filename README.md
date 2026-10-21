# Telcom Revenue at Risk Prediction

## Overview

This project uses machine learning to predict customer churn probabilities and estimate revenue exposure associated with customers who may leave a telecommunications service provider.

The project introduces **Feedback-Adjusted Revenue-at-Risk (FARR)**, an exploratory metric that combines monthly customer charges, predicted churn probabilities, and a feedback-risk score.

## Objectives

- Explore and understand the customer dataset.
- Analyse historical churn and revenue exposure.
- Train and evaluate churn classification models.
- Estimate customer-level churn probabilities.
- Calculate and compare predicted FARR across customer segments.
- Translate model outputs into actionable customer-retention insights.

## Methodology

1. Data quality assessment and exploratory data analysis.
2. Feature preparation and preprocessing.
3. Baseline model development.
4. Model training and evaluation.
5. Predicted FARR calculation and segment comparison.
6. Documentation of findings, limitations, and recommendations.

## Technology Stack

- Python
- pandas and NumPy
- scikit-learn
- Matplotlib and Seaborn
- Jupyter
- pytest
- Ruff
- Git and GitHub

## Project Structure

- `data/` — local datasets
- `notebooks/` — exploratory analysis and experiments
- `src/farr/` — reusable project code
- `tests/` — automated tests
- `docs/` — methodology and technical documentation
- `models/` — model artifacts
- `reports/` — generated figures and reports

## Evaluation

Classification models will be evaluated using appropriate metrics such as precision, recall, F1-score, ROC-AUC, and probability calibration.

Predicted FARR will be interpreted as an exploratory, feedback-weighted revenue-exposure indicator. It is not a guarantee of future revenue loss.

## Data and Reproducibility

Dataset provenance, preprocessing decisions, experimental configurations, and results will be documented as the project progresses.

Raw datasets and generated artifacts are not intended to be committed to GitHub by default.

## Project Status

**Status:** Initial setup

The development environment and project structure are being established. Data analysis and model development have not yet been completed.