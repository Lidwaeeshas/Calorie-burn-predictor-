# Calories Burned Prediction with Regression Models

## 📌 Overview
This project predicts **calories burned** during exercise using various **regression techniques** and evaluates their performance with multiple diagnostic checks.  
It demonstrates a **full end-to-end machine learning pipeline** — from data preprocessing to model evaluation — using **Linear Regression, Ridge, Lasso, and ElasticNet**.


## 🗂 Dataset
The dataset (`train.csv`) contains features such as:
- **Sex** (encoded as binary)
- **Age**
- **Height**
- **Weight**
- **Duration** of activity
- **Heart Rate**
- **Body Temperature**
- **Calories burned** (target variable)


## ⚙ Features of This Project
- **Data Cleaning & Preprocessing**
  - Encoding categorical variables
  - Removing duplicates
  - Outlier detection with IQR method
  - Target transformation (square root scaling)
  - Standardization with `StandardScaler`
- **Model Training**
  - Linear Regression
  - Ridge Regression (GridSearchCV tuning)
  - Lasso Regression (GridSearchCV tuning)
  - ElasticNet Regression (GridSearchCV tuning)
- **Statistical Diagnostics**
  - **Linearity & Homoscedasticity** checks
  - **Independence** test using Durbin-Watson
  - **Multicollinearity** check via Variance Inflation Factor (VIF)
  - **Normality** check for residuals
- **Evaluation Metrics**
  - R² Score
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - Mean Absolute Error (MAE)
  - F-statistic and p-values from Statsmodels

## 📊 Model Evaluation
Example outputs:
```python
{
    "r2": 0.89,
    "mse": 1.45,
    "root mean square": 1.20,
    "mean absolute error": 0.85,
    "coefficients": {...},
    "p value": 1.23e-10
}
