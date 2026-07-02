# Telco Customer Churn Prediction

## Overview

Customer churn is one of the biggest challenges faced by telecom companies. Retaining existing customers is often more cost-effective than acquiring new ones. This project aims to predict whether a customer is likely to leave the telecom service using Machine Learning.

A Logistic Regression model was trained on the Telco Customer Churn dataset to classify customers as likely to churn or not churn.

---

## Dataset

Dataset Source: Telco Customer Churn Dataset

* Total Records: 7043
* Features: Customer demographics, account information, services subscribed, billing details
* Target Variable: Churn (Yes/No)

---

## Project Workflow

### 1. Data Cleaning

* Removed customerID column
* Converted TotalCharges to numeric format
* Handled missing values using median imputation
* Removed duplicate records
* Standardized categorical values

### 2. Exploratory Data Analysis (EDA)

* Churn Distribution Analysis
* Contract Type vs Churn
* Monthly Charges vs Churn
* Tenure Analysis
* Customer Service Feature Analysis

### 3. Data Preprocessing

* One-Hot Encoding for categorical variables
* Feature Scaling using StandardScaler
* Train-Test Split (80:20)

### 4. Model Training

* Logistic Regression Classifier

### 5. Model Evaluation

* Accuracy Score
* Precision
* Recall
* F1 Score
* Confusion Matrix
* ROC-AUC Score

---

## Results

### Model Performance

| Metric            | Score |
| ----------------- | ----- |
| Accuracy          | 80.3% |
| Precision (Churn) | 66%   |
| Recall (Churn)    | 53%   |
| F1-Score (Churn)  | 59%   |

Confusion Matrix:

| Actual / Predicted | No Churn | Churn |
| ------------------ | -------- | ----- |
| No Churn           | 932      | 101   |
| Churn              | 176      | 196   |

---

## Key Business Insights

* Customers with month-to-month contracts are more likely to churn.
* Customers with shorter tenure show higher churn rates.
* Higher monthly charges are associated with increased churn probability.
* Long-term contracts significantly reduce churn.
* Additional services such as Tech Support and Online Security improve customer retention.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

---

## Future Improvements

* Random Forest Classifier
* XGBoost Classifier
* Hyperparameter Tuning
* Feature Selection
* Model Deployment using Streamlit or Flask

---

## Author

Vansh Garg

B.Tech CSE (Artificial Intelligence)

Machine Learning and Data Science Enthusiast
