# Customer Churn Prediction for Telecom

## Business Context

Telecommunication companies operate in a highly competitive market where customer retention is critical to sustaining revenue and growth. Acquiring new customers is often more expensive than retaining existing ones, making it essential for companies to understand customer behavior and proactively reduce churn.

---

# Problem Statement

Customer churn refers to customers who stop using a company’s service or switch to a competitor due to factors such as pricing, poor customer experience, service dissatisfaction, or better alternatives.

In the telecom industry, customer churn directly affects:
- revenue generation,
- customer lifetime value,
- and long-term business stability.

Understanding why customers leave helps companies improve retention strategies and customer satisfaction.

---

# Project Objective

The goal of this project is to analyze telecom customer behavior, identify key churn drivers, and prepare a machine-learning-ready dataset for predictive modeling.

The project combines:
- exploratory data analysis (EDA),
- feature engineering,
- preprocessing,
- and machine learning techniques

to support churn prediction and customer retention strategies.

---

# Dataset Information

The dataset contains telecom customer information including:
- demographic details,
- account information,
- subscribed services,
- billing information,
- and churn status.

### Target Variable
- `churn`

---

# Exploratory Data Analysis (EDA)

The EDA phase focused on understanding customer behavior patterns, identifying churn drivers, and uncovering relationships between customer attributes and churn status.

---

# Univariate Analysis

The following numerical features were analyzed:
- tenure
- monthlycharges
- totalcharges

### Major Findings
- Most churned customers exhibit low tenure.
- Higher monthly charges are associated with increased churn behavior.
- Retained customers generally accumulate higher total charges over time.

Categorical feature analysis also revealed important churn patterns across:
- contract type,
- internet service,
- payment methods,
- support services,
- and security-related features.

---

# Bivariate and Multivariate Analysis

Further analysis revealed several important churn patterns:

### Contract Type
- Month-to-month customers exhibit the highest churn rates.
- Long-term contract customers are generally more stable.

### Internet Service
- Fiber optic customers show higher churn compared to DSL users.
- Some fiber customers remain subscribed for long periods before eventually churning.

### Support and Protection Services
Customers without:
- tech support,
- online security,
- online backup,
- or device protection

consistently exhibit higher churn behavior.

### Payment Method
- Electronic check users show significantly higher churn.
- Automatic payment methods are associated with lower churn risk.

---

# Correlation Analysis

Phik correlation analysis was performed to measure relationships between both numerical and categorical variables.

### Features Most Associated with Churn
- tenure
- paymentmethod
- monthlycharges
- paperlessbilling
- contract
- techsupport
- onlinesecurity

### Features With Weak Relationship to Churn
- gender
- phoneservice

The analysis indicates that customer churn is influenced by multiple behavioral, pricing, and service-related factors rather than a single variable.

---

# Feature Engineering & Preprocessing

The dataset was transformed into a machine-learning-ready format through several preprocessing steps:

### Preprocessing Steps
- Feature and target separation
- Binary feature encoding
- One-hot encoding of categorical variables
- Train-test splitting using stratified sampling
- Feature scaling using `RobustScaler`
- Class imbalance handling using `SMOTE`

### Additional Engineering Decisions
- `customerid` was removed due to lack of predictive value.
- Outlier analysis was performed without aggressive removal to preserve valid high-value customers.
- Both baseline and SMOTE-balanced training datasets were retained for model comparison.

### Final Prepared Datasets
- `X_train`
- `X_test`
- `y_train`
- `y_test`
- `X_train_smote`
- `y_train_smote`

---

# Tools and Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Phik
- Jupyter Notebook

---

# Project Structure

```bash
Customer-churn-ML/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── EDA.ipynb
│   └── Feature_Engineering.ipynb
│
├── README.md
├── metadata.md
├── LICENSE
└── .gitignore

---
# Conclusion

The analysis identified several important drivers of customer churn, including customer tenure, pricing structure, contract type, billing behavior, and support-related services.

The preprocessing pipeline successfully transformed the dataset into a machine-learning-ready format while preserving important business information and addressing class imbalance challenges.

These insights and engineered datasets provide a strong foundation for developing predictive machine learning models capable of identifying high-risk customers and supporting proactive retention strategies