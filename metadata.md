# Dataset Metadata: Telco Customer Churn

## Overview

This dataset contains customer-level information for a telecom company, including demographics, account details, service usage, and churn status. It is used to analyze and predict customer churn behavior.

---

## Feature Description

### Customer Information

* **customerID**: Unique identifier for each customer

---

### Demographics

* **gender**: Gender of the customer (Male, Female)
* **SeniorCitizen**: Whether the customer is a senior citizen (1 = Yes, 0 = No)
* **Partner**: Whether the customer has a partner (Yes, No)
* **Dependents**: Whether the customer has dependents (Yes, No)

---

### Account Information

* **tenure**: Number of months the customer has stayed with the company
* **Contract**: Type of contract (Month-to-month, One year, Two year)
* **PaperlessBilling**: Whether the customer uses paperless billing (Yes, No)
* **PaymentMethod**: Payment method used by the customer

---

### Services Subscribed

* **PhoneService**: Whether the customer has phone service (Yes, No)

* **MultipleLines**: Whether the customer has multiple lines (Yes, No, No phone service)

* **InternetService**: Type of internet service (DSL, Fiber optic, No)

* **OnlineSecurity**: Whether the customer has online security (Yes, No, No internet service)

* **OnlineBackup**: Whether the customer has online backup (Yes, No, No internet service)

* **DeviceProtection**: Whether the customer has device protection (Yes, No, No internet service)

* **TechSupport**: Whether the customer has tech support (Yes, No, No internet service)

* **StreamingTV**: Whether the customer has streaming TV (Yes, No, No internet service)

* **StreamingMovies**: Whether the customer has streaming movies (Yes, No, No internet service)

---

### Financial Information

* **MonthlyCharges**: Monthly amount charged to the customer
* **TotalCharges**: Total amount charged to the customer

---

### Target Variable

* **Churn**: Whether the customer left the company (Yes = churned, No = retained)

---

