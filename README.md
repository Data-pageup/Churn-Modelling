# Churn Prediction Workflows

## Overview
This repo contains two quick churn prediction workflows built with **LogisticRegressionCV**.  
The goal was to revisit end-to-end ML steps — data handling, visualization, and modeling — in ~20 minutes.

## Workflows
### 1. Bank Customer Churn
- **Dataset**: Customer info (CreditScore, Geography, Gender, Age, Tenure, Balance, NumOfProducts, HasCrCard, IsActiveMember, EstimatedSalary, Exited).
- **Steps**:
  - Preprocessing: one-hot encoding for categorical features, scaling numerical features.
  - Visualization: countplots, boxplots, scatterplots to explore churn patterns.
  - Modeling: LogisticRegressionCV with 5-fold CV, auto-tuned regularization.
  - Feature Importance: plotted coefficients to interpret churn drivers.

### 2. Telecom Churn
- **Dataset**: Call records (Failures, Complains, Subscription, Length, Charge, Amount, Seconds of Use).
- **Steps**:
  - Preprocessing: cleaned columns, scaled features.
  - Visualization: churn distribution and feature relationships.
  - Modeling: LogisticRegressionCV with cross-validation.
  - Feature Importance: coefficient plot to highlight key predictors.

## Tech Stack
- Python 3.x
- pandas, numpy
- matplotlib, seaborn
- scikit-learn (LogisticRegressionCV, train_test_split, StandardScaler)

## Results
- Both workflows ran end-to-end successfully.
- LogisticRegressionCV automatically selected the best `C` value.
- Feature importance visualizations provided interpretable insights into churn drivers.

### Amirtha Ganesh R
