# Customer Churn Prediction Using Machine Learning

## Project Overview

This project focuses on predicting customer churn for a telecommunications company using Machine Learning techniques. The goal is to identify customers who are likely to discontinue their services so that the company can take proactive retention measures.

The project covers a complete end-to-end machine learning workflow including:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Handling Imbalanced Data using SMOTE
- Model Building
- Model Evaluation
- Hyperparameter Tuning
- Feature Importance Analysis
- Business Insights & Recommendations

The final selected model was:

**Gradient Boosting (SMOTE)**

---

# Business Problem

Customer churn is a major challenge in the telecommunications industry because acquiring new customers is often more expensive than retaining existing ones.

The objective of this project is to build a machine learning model capable of predicting customers who are likely to churn based on customer demographics, account information, subscribed services, and payment behavior.

---

# Dataset Information

The dataset contains customer-related information such as:

- Customer demographics
- Contract type
- Payment method
- Internet services
- Monthly charges
- Customer tenure
- Churn status

### Target Variable

- `Churn`

---

# Project Workflow

## 1. Data Cleaning & Preprocessing

The following preprocessing steps were performed:

- Handled missing values
- Converted categorical variables
- Feature encoding using One-Hot Encoding
- Feature scaling where necessary
- Removed data inconsistencies

---

## 2. Exploratory Data Analysis (EDA)

EDA was conducted to understand:

- churn distribution
- customer behavior patterns
- relationships between variables and churn
- important business trends

Several visualizations were created using:

- Matplotlib
- Seaborn

### Key Findings

- Customers with month-to-month contracts showed higher churn tendencies.
- Customers with shorter tenure were more likely to churn.
- Fiber optic internet users showed relatively higher churn behavior.
- Customers using electronic check payment methods had higher churn tendencies.
- Additional services such as online security and tech support improved customer retention.

---

## 3. Handling Imbalanced Data

The dataset contained class imbalance in the target variable.

To address this issue:

**SMOTE (Synthetic Minority Oversampling Technique)** was applied to balance the churn classes and improve model learning.

---

# Machine Learning Models Used

The following classification models were trained and evaluated:

- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
- AdaBoost
- XGBoost
- LightGBM
- CatBoost
- Support Vector Classifier (SVC)
- K-Nearest Neighbors (KNN)
- SGD Classifier

Both:

- baseline models
- SMOTE-enhanced models

were compared.

---

# Model Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score
- Confusion Matrix
- ROC Curve Analysis

---

# Hyperparameter Tuning

RandomizedSearchCV was used for hyperparameter optimization on the top-performing models:

- Gradient Boosting
- AdaBoost
- Logistic Regression
- SVC

The tuned and untuned models were compared to evaluate performance improvements.

The untuned Gradient Boosting (SMOTE) model ultimately provided better overall balance and generalization performance.

---

# Final Model Selection

After comparing all trained models, the:

## Gradient Boosting (SMOTE)

model was selected as the final model because it provided the best balance between:

- Recall
- Precision
- F1-Score
- ROC-AUC
- Generalization Performance

### Final Model Performance

| Metric | Score |
|---|---|
| Accuracy | 0.7736 |
| Precision | 0.5565 |
| Recall | 0.7246 |
| F1-Score | 0.6295 |
| ROC-AUC | 0.8396 |

---

# Feature Importance Analysis

Feature importance analysis revealed that the most influential factors affecting customer churn were:

- Contract Type
- Customer Tenure
- Internet Service Type
- Payment Method
- Online Security
- Tech Support
- Monthly Charges

The analysis showed that customers with short-term contracts and shorter tenure were more likely to churn.

---

# Key Business Insights

- Customers on month-to-month contracts are more likely to churn.
- Long-term contracts improve customer retention.
- New customers have higher churn tendencies.
- Fiber optic internet customers showed higher churn risk.
- Customers using electronic check payment methods were more likely to churn.
- Additional support services such as tech support and online security contributed positively to customer retention.

---

# Business Recommendations

Based on the findings, the following recommendations are proposed:

- Encourage customers to adopt long-term contracts.
- Improve onboarding and engagement for new customers.
- Investigate customer experience among fiber optic users.
- Promote automated payment methods.
- Expand value-added support services.

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)
- XGBoost
- LightGBM
- CatBoost
- Joblib

---

# Project Structure

```bash
Customer-Churn-ML/
│
├── data/
├── notebooks/
├── models/
├── visuals/
├── README.md
└── requirements.txt
```

---

# Model Saving

The final trained model was saved using:

```python
joblib
```

Saved files:

- customer_churn_gradient_boosting.pkl
- model_features.pkl

---

# Future Improvements

Possible future enhancements include:

- Model deployment using Streamlit or Flask
- SHAP explainability integration
- Advanced feature engineering
- Ensemble model stacking

---

# Conclusion

This project successfully developed a machine learning solution capable of predicting customer churn with strong predictive performance.

The findings from this project can help businesses:

- identify high-risk customers
- improve retention strategies
- reduce customer loss
- improve customer satisfaction
- support data-driven decision-making
