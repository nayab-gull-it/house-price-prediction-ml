# House Price Prediction using ML

## Overview
This project performs exploratory data analysis (EDA) on a house price dataset, followed by data visualization and training multiple regression models to predict house prices based on features like area, bedrooms, location score, and more.

## Objective
Predict house prices accurately using property features, and compare multiple regression algorithms to identify the best-performing model.

## Tools & Libraries
Python · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn

## Key Steps
1. Exploratory Data Analysis (distributions, correlations, outliers)
2. Data visualization of key price-driving features
3. Feature engineering and preprocessing
4. Training and comparing multiple regression models:
   - Linear Regression
   - Ridge Regression
   - Lasso Regression
   - Random Forest Regressor
   - Gradient Boosting Regressor
5. Hyperparameter tuning via GridSearchCV (5-fold cross-validation)

## Results
**Best Model:** Gradient Boosting Regressor

| Metric | Score |
|---|---|
| R² Score | 0.894 |
| Best CV R² Score (tuned) | 0.913 |
| RMSE | 74,701.34 |
| MAE | 39,862.80 |

**Best Hyperparameters:**
`learning_rate: 0.05, max_depth: 2, n_estimators: 300, subsample: 0.8`

## Key Findings
- Gradient Boosting outperformed Linear, Ridge, Lasso, and Random Forest models, achieving the strongest fit after hyperparameter tuning.
- Cross-validation confirmed the tuned model generalizes well (CV R² of 0.913 vs standalone R² of 0.894), indicating low overfitting risk.
- Hyperparameter tuning improved performance meaningfully over default settings, highlighting the value of systematic search (GridSearchCV) over manual tuning.

## Notebook
[View full notebook on Kaggle](https://www.kaggle.com/code/nayabgulll964/hpp-using-ml-by-nayab-gull)
