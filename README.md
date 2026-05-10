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

The goal of this project is to analyze telecom customer behavior and identify the major factors associated with customer churn using exploratory data analysis (EDA).

The insights generated from this analysis will later support the development of a machine learning churn prediction model.

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

# Key Business Insights

- Early-stage customers are the most vulnerable to churn.
- High-paying customers may leave when service expectations are not met.
- Long-term contracts improve customer stability.
- Technical support and security services improve retention.
- Customers integrated into multiple services tend to exhibit lower churn behavior.
- Automatic payment methods are associated with lower churn risk.

---

# Tools and Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Phik
- Jupyter Notebook

---

# Project Structure

```bash
Customer-churn-ML/
│
├── data/
│   └── telco_churn.csv
│
├── notebooks/
│   └── EDA.ipynb
│
├── README.md
├── metadata.md
├── LICENSE
└── .gitignore
```

---

# Current Project Status

✅ Data cleaning completed  
✅ Exploratory data analysis completed  
✅ Correlation analysis completed  

🚧 Feature engineering and machine learning phases are currently in progress.

---

# Conclusion

The exploratory analysis successfully identified several key factors associated with customer churn, including customer tenure, pricing structure, contract type, billing behavior, and support-related services.

The insights from this phase provide a strong foundation for building future machine learning models capable of identifying high-risk customers and supporting proactive retention strategies.