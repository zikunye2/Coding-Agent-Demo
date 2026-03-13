# Customer Churn Prediction

## Overview
Built a complete machine learning pipeline to predict customer churn for a telecom company using the IBM Telco Customer Churn dataset (~7,000 customers, 21 features).

## Methods
- **XGBoost Classifier**: Gradient boosting model with 100 estimators
- **Feedforward Neural Network (PyTorch)**: 2 hidden layers (64→32 neurons), ReLU activation, Dropout regularization

## Key Findings
- **Top churn drivers**: tenure (length of service), Contract type (month-to-month vs. long-term), MonthlyCharges, InternetService (fiber optic), and TechSupport
- Both models achieved strong predictive performance (AUC-ROC > 0.80)
- XGBoost provided better interpretability through feature importance rankings

## Business Recommendations
1. **Target month-to-month customers**: Offer incentives to switch to annual or two-year contracts, as contract type is a top churn predictor
2. **Early engagement programs**: Customers with short tenure are at highest risk — implement onboarding campaigns within the first 6 months
3. **Review fiber optic pricing**: Fiber optic customers churn at higher rates, possibly due to higher monthly charges — consider competitive pricing or bundled discounts

## Skills Used
Python, XGBoost, PyTorch, scikit-learn, pandas, matplotlib, seaborn
