# Customer Churn Prediction

## Overview
A machine learning project to predict customer churn using classification algorithms and ensemble learning techniques. The goal is to identify customers likely to leave a subscription based service so the business can take proactive retention action.

## Dataset
Telco Customer Churn dataset (WA_Fn-UseC_-Telco-Customer-Churn.csv)

## Workflow
1. Data loading and exploratory data analysis (EDA)
2. Data preprocessing (encoding, scaling, train-test split)
3. Individual model training: Logistic Regression, KNN, Decision Tree, Naive Bayes, SVM
4. Ensemble methods: Voting, Bagging, AdaBoost, Gradient Boosting, Stacking
5. Hyperparameter tuning with GridSearchCV
6. Final model evaluation (confusion matrix, classification report, feature importance)

## Results
| Model | Accuracy |
|---|---|
| Voting Ensemble | 0.8226 |
| Stacking | 0.8219 |
| AdaBoost | 0.8141 |
| Tuned Gradient Boosting | 0.8126 |
| Gradient Boosting | 0.8119 |
| Bagging | 0.7750 |

**Best Model:** Voting Ensemble — 82.26% Accuracy

## Key Insights
- Contract type, tenure, and monthly charges are the strongest churn predictors
- Month to month contract customers churn at a much higher rate
- Customers without internet service show the lowest churn rate
- Ensembles combining diverse algorithms (Voting, Stacking) outperformed single algorithm ensembles (Bagging, Boosting)

## Tech Stack
Python, Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib


