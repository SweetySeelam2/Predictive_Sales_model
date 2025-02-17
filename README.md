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

## Conclusion
=> Model Comparison
Random Forest MAE: 9.21
XGBoost MAE: 8.66
XGBoost outperforms Random Forest with a lower Mean Absolute Error (MAE), making better predictions.
=> Feature Importance (SHAP Analysis)
Top Influential Features:
Rolling Mean (7-day average sales): Has the highest impact on predictions.
Sales Lag Features (7, 14, 30 days): Past sales data significantly influence future predictions.
Day of the Week & Month: Sales trends vary based on weekdays and months.
Holiday Indicator: Sales tend to fluctuate around holidays.
=> Observations from SHAP Plot
Features with higher SHAP values have a greater influence on model predictions.
Rolling Mean & Recent Sales Lags dominate the prediction, highlighting the importance of time-series patterns.
=> Key Takeaways
- XGBoost performs better than Random Forest, making it the preferred model.
- Sales prediction is highly dependent on historical sales trends.
- Time-related factors like week, month, and holiday status play an essential role in forecasting sales.

## Deployment & Usage
```bash
git clone https://github.com/your-username/Predictive-Sales-Model.git
cd Predictive-Sales-Model
streamlit run app.py
