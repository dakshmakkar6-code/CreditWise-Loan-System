# CreditWise – Intelligent Loan Approval System

## Project Overview

CreditWise is a Machine Learning–powered loan approval prediction system designed for SecureTrust Bank, a mid-sized financial institution processing personal and home loans across urban and rural regions of India.

Traditionally, the bank relied on a manual verification process where loan officers reviewed income proofs, employment details, credit history, and supporting documents. This process was:

- Time-consuming  
- Prone to human bias  
- Inconsistent across applications  

As a result, the bank faced two major challenges:

1. Creditworthy applicants were sometimes rejected (loss of business)
2. High-risk applicants were sometimes approved (financial risk)

This project builds an intelligent decision-support system that predicts whether a loan should be **Approved (1)** or **Rejected (0)** using historical loan application data.

The model is intended to assist human officers by providing faster, more consistent, and data-driven insights before final verification.

---

## Objective

Develop a supervised machine learning classification model that:

- Learns patterns from historical loan data
- Minimises false approvals (reduce financial risk)
- Minimises false rejections (retain good customers)
- Improves decision consistency
- Supports data-driven financial decision-making

---

## Dataset Description

Each row represents a loan applicant and includes personal, financial, and credit-related attributes.

### Personal Information
- Applicant_ID
- Age
- Gender
- Marital_Status
- Dependents
- Education_Level

### Employment & Financial Information
- Applicant_Income
- Coapplicant_Income
- Employment_Status (Salaried / Self-Employed / Business)
- Employer_Category (Govt / Private / Self)
- Savings
- Existing_Loans
- DTI_Ratio (Debt-to-Income Ratio)
- Credit_Score

### Loan & Property Information
- Loan_Amount
- Loan_Term (in months)
- Loan_Purpose (Home / Education / Personal / Business)
- Property_Area (Urban / Semi-Urban / Rural)
- Collateral_Value

### Target Variable
- Loan_Approved  
  - 1 = Approved  
  - 0 = Rejected  

---

## Machine Learning Approach

This project follows an end-to-end ML workflow:

### Data Understanding
- Dataset loading
- Exploratory analysis
- Checking data structure and missing values

### Data Preprocessing
- Handling missing values
- Encoding categorical variables
- Feature scaling using StandardScaler
- Train-test split for proper evaluation

### Model Building
- Logistic Regression (baseline classification model)

### Model Evaluation
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

These metrics help analyse both:
- False Positives (risk exposure)
- False Negatives (missed good customers)

---

## Current Model (v1)

- Model: Logistic Regression, KNN, Naive Bayes
- Data split: Train/Test
- Feature scaling applied
- Performance evaluated using multiple classification metrics

This version establishes a strong baseline model for structured loan risk prediction.

---

## Business Interpretation

- High recall helps reduce the rejection of creditworthy applicants.
- High precision helps prevent high-risk applicants from being approved.
- The model serves as a decision-support tool rather than a full automation system.

It is designed to assist human verification, not replace it.

---

## Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Future Improvements

This repository will evolve through iterative improvements:

- Implement Scikit-learn Pipeline
- Add Random Forest and ensemble model comparison
- Feature importance analysis
- Hyperparameter tuning
- Cross-validation
- Model explainability (SHAP / feature interpretation)
- Deployment using Streamlit

## 📁 Dataset

The dataset used in this project is included in the `/data` folder
for reproducibility and demonstration purposes.

