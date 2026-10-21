# Project Methodology

## 1. Business Problem

Customer churn can expose a telecommunications provider to potential
recurring revenue loss. The project aims to estimate this exposure and
identify customer segments that may warrant retention attention.

## 2. Churn Prediction

Train classification models using customer attributes as input features
and historical churn as the target.

Candidate models:
- Logistic Regression
- Random Forest Classifier

Model selection will be based on held-out evaluation rather than
training performance alone.

## 3. Feedback-Adjusted Revenue-at-Risk (FARR)

The proposed metric combines monthly charges, estimated churn
probability, and a feedback-risk score.

For customer segment s:

FARR_hat_s =
100 * sum(M_i * P_hat_i * (1 + F_i))
      / sum(M_i)

Where:
- M_i: monthly charges for customer i.
- P_hat_i: predicted probability of churn.
- F_i: feedback-risk score, whose definition and range must be documented.
- s: customer segment.

## 4. Evaluation

Evaluate classification using appropriate metrics, including precision,
recall, F1-score, ROC-AUC, and probability calibration.

Compare predicted FARR across segments and examine how sensitive the
results are to the feedback-risk weighting.

## 5. Limitations

FARR is an exploratory metric, not a standard financial risk measure.
Its interpretation depends on the validity of the feedback score and
the chosen weighting formula.

A customer-level dataset without repeated time periods cannot by itself
establish that the model forecasts future revenue loss over time.
