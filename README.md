# Predictive Sales Model

## Project Overview
This project develops a Predictive Sales Model to forecast sales revenue for a retail store using machine learning (Random Forest &amp; XGBoost) and advanced feature engineering. The model is designed to optimize business decisions by predicting future sales based on historical data.

## Key Features:
Dataset: Retail Store Sales Transactions (Kaggle: https://www.kaggle.com/datasets/marian447/retail-store-sales-transactions)
-Regular Model: Random Forest
-Advanced Model: XGBoost with hyperparameter tuning
-Feature Engineering: Lag variables, rolling averages, holiday effects
-Model Explainability: SHAP for feature interpretation
-Deployment: Streamlit & Flask API

## Model Performance
| Model | R² Score | RMSE |
|-------|---------|------|
| Random Forest | 0.92 | 150.23 |
| XGBoost | 0.95 | 130.45 |

## Deployment & Usage
```bash
git clone https://github.com/your-username/Predictive-Sales-Model.git
cd Predictive-Sales-Model
streamlit run app.py
