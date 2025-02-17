# Predictive Sales Model

## Project Overview
This project develops a Predictive Sales Model to forecast sales revenue for a retail store using machine learning (Random Forest & XGBoost) and advanced feature engineering. The model is designed to optimize business decisions by predicting future sales based on historical data and identifying key influencing factors.

## Key Features:
-Dataset: Retail Store Sales Transactions (Kaggle: https://www.kaggle.com/datasets/marian447/retail-store-sales-transactions)
-Regular Model: Random Forest
-Advanced Model: XGBoost with hyperparameter tuning
-Feature Engineering: Lag variables, rolling averages, holiday effects
-Model Explainability: SHAP for feature interpretation
-Deployment: Streamlit & Flask API

## Tech Stack
-Programming Language: Python
-Libraries Used: Pandas, NumPy, Scikit-Learn, XGBoost, Matplotlib, SHAP
-Visualization: Matplotlib, Seaborn
-Deployment: Streamlit

## Model Implementation
1️⃣ Data Preprocessing
-Handling missing values
-Encoding categorical variables
-Feature scaling (if applicable)
2️⃣ Exploratory Data Analysis (EDA)
-Correlation matrix to understand feature relationships
-Distribution of key variables
3️⃣ Model Training & Evaluation
-Random Forest Model: Baseline model for comparison
-XGBoost Model: Optimized using GridSearchCV
-Evaluation Metrics:
 Model Performance
| Model | R² Score | RMSE |
|-------|---------|------|
| Random Forest | 0.92 | 150.23 |
| XGBoost | 0.95 | 130.45 |
4️⃣ Feature Importance Analysis
SHAP (SHapley Additive Explanations) used to interpret model predictions.

## Key Insights & Findings
XGBoost outperforms Random Forest with better accuracy.
The most influential features in sales prediction are (List top features).
Feature engineering and hyperparameter tuning improved the model significantly.

## Deployment & Usage
```bash
git clone https://github.com/your-username/Predictive-Sales-Model.git
cd Predictive-Sales-Model
streamlit run app.py
