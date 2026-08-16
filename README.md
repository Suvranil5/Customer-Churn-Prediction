# Customer Churn Prediction

## Project Overview

Customer churn is a major business challenge for subscription-based companies. This project analyzes customer demographics, services, contracts, tenure, and billing information to identify factors associated with customer churn and build machine learning models to predict customers at risk of leaving.

The project combines exploratory data analysis, feature preprocessing, classification models, model evaluation, and business recommendations.

## Objectives

- Analyze customer churn patterns.
- Identify customer characteristics associated with churn.
- Explore relationships between contracts, services, tenure, and billing and churn.
- Prepare customer data for machine learning.
- Build and compare multiple churn prediction models.
- Identify important churn drivers.
- Provide actionable customer-retention recommendations.

## Dataset

The project uses a telecommunications customer churn dataset containing customer demographic, service, contract, and billing information.

The dataset contains approximately 7,000 customer records and includes the target variable `Churn Label`.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook
- VS Code
- Git & GitHub

## Project Workflow

1. Data loading and inspection
2. Data quality assessment
3. Exploratory data analysis
4. Churn distribution analysis
5. Customer segment analysis
6. Feature and target separation
7. Train-test split
8. Feature preprocessing
9. Logistic Regression
10. Decision Tree
11. Random Forest
12. Model evaluation
13. Model comparison
14. Feature importance analysis
15. Business recommendations

## Models Evaluated

### Logistic Regression

Used as the baseline classification model because it provides an interpretable benchmark for binary churn prediction.

### Decision Tree

Used to capture non-linear relationships and interactions between customer characteristics.

### Random Forest

Used as an ensemble model combining multiple decision trees to improve predictive stability and overall performance.

## Model Performance

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 80.20% | 64.35% | 56.95% | 60.43% | 84.89% |
| Decision Tree | 79.42% | 61.60% | 59.63% | 60.60% | 83.53% |
| Random Forest | 80.70% | 66.78% | 54.28% | 59.88% | 85.34% |

Random Forest achieved the highest ROC-AUC and accuracy among the three evaluated models, while the Decision Tree achieved the highest recall.

## Key Business Insights

- Month-to-month customers show substantially higher churn than customers on longer-term contracts.
- Fiber-optic customers demonstrate elevated churn compared with other internet-service groups.
- Customers with higher recurring charges show greater churn risk.
- Customers without services such as online security and technical support show higher churn rates.
- Predictive modeling can help prioritize customers for targeted retention campaigns.

## Business Recommendations

- Encourage month-to-month customers to move to longer-term contracts through targeted incentives.
- Investigate pricing and perceived-value concerns among customers with higher monthly charges.
- Develop targeted retention strategies for high-risk internet-service segments.
- Consider bundled security and technical-support offerings.
- Use churn probabilities to prioritize customers for proactive retention campaigns.
- Consider threshold tuning when maximizing churner identification is more important than overall accuracy.

## Repository Structure

```text
Customer-Churn-Prediction/
│
├── data/
│   └── Telco_customer_churn.xlsx
│
├── notebooks/
│   └── customer_churn_analysis.ipynb
│
├── visuals/
│
└── README.md