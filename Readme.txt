# Credit Lending Strategy Enhancement: A Machine Learning Approach

## Level 01: Current Challenge Faced by the Bank
### Problem Statement
The bank faces challenges in assessing credit risk effectively, leading to suboptimal lending decisions. This project aims to enhance the credit lending strategy using a more scientific, data-driven approach.

### Dataset Overview
1. **Bureau Dataset**:
   - Contains credit-related information from external financial institutions.
   - Features include:
     - Loan types
     - Repayment history
     - Defaults
     - Credit utilization ratio

2. **Internal Product Dataset**:
   - Contains internal data related to the bank's existing products.
   - Features include:
     - Customer demographics
     - Internal credit scoring
     - Product-specific repayment details

### Features Explanation
- Loan Amount
- Interest Rate
- Credit Tenure
- Customer Income
- Existing Loan Count
- Default Flag (binary indicator of default)

### Target Variable
- **Multiclass Risk Categories**:
  - Low Risk
  - Medium Risk
  - High Risk
- Objective: Understand the risk appetite and categorize customers accordingly.

### Objective of ML Modelling
- To revise the current credit lending strategy with a scientific, data-driven model that assesses creditworthiness accurately.

### Proposed Solution
- Utilize machine learning models to:
  - Predict credit risk categories.
  - Optimize lending decisions.
  - Enhance financial outcomes by reducing Non-Performing Assets (NPAs).

---

## Level 02: Banking and Credit Risk Basics

### Types of Credit Risks
1. **Default Risk**: Borrowers' inability to repay.
2. **Concentration Risk**: Overexposure to specific sectors or borrowers.
3. **Liquidity Risk**: Inability to meet short-term obligations.

### Banking Basics
- **Asset vs Liability**:
  - Assets: Loans, investments.
  - Liabilities: Deposits, borrowings.
- **Net Interest Margin (NIM)**:
  - Difference between interest earned and interest paid.
- **Gross NPA vs Net NPA**:
  - GNPA: Total non-performing loans.
  - NNPA: GNPA adjusted for provisions.

### Corporate Data Science Workflow
1. **Roles**:
   - ML Engineers
   - MLOps Specialists
   - Data Engineers
   - Product Managers
2. **Steps**:
   - Data collection and cleaning.
   - Model development.
   - Deployment and monitoring.

### FAQs for Data Science Interviews
- Explain feature selection techniques.
- How do you handle imbalanced datasets?
- What is the significance of hyperparameter tuning?

---

## Level 03: Data Preparation and Modelling

### Data Preparation
1. **Joining Datasets**:
   - Combine Bureau and Internal datasets on a common identifier.
2. **Data Cleaning**:
   - Handle null values (imputation).
   - Remove outliers (z-score, IQR).

### Exploratory Data Analysis (EDA)
- Identify trends and patterns.
- Visualize relationships between features and the target variable.

### Feature Engineering
1. **Tests for Feature Selection**:
   - Chi-Square Test
   - ANOVA
2. **Multicollinearity**:
   - Check using Variance Inflation Factor (VIF).
3. **Encoding**:
   - Label Encoding
   - One-Hot Encoding

### Model Selection
- Choose models such as Random Forest, XGBoost, or Logistic Regression.
- Evaluate using appropriate loss metrics (e.g., log loss, F1-score).

### Hyperparameter Tuning
- Use Grid Search or Random Search for optimization.

---

## Level 04: Model Analysis and Deployment

### Model Analysis
- Evaluate model results on validation data.
- Analyze metrics like Accuracy, Precision, Recall, and AUC-ROC.

### Deployment
1. Deploy the model into the bank's production environment.
2. Configure a feedback loop to collect insights from bank employees.

### Retraining
- Incorporate feedback from end-users.
- Retrain the model periodically to improve performance.

### Explaining Model Results
- Simplify complex metrics into business terms.
- Use visualizations to demonstrate insights (e.g., customer risk distribution).

---

## Repository Structure
```
credit-lending-strategy/
|
├── data/                   # Datasets (Bureau, Internal Product)
├── notebooks/              # Jupyter Notebooks for EDA, Feature Engineering
├── models/                 # Saved ML models
├── src/                    # Source code for model training and deployment
├── reports/                # Analysis and documentation
└── README.md               # Project overview and instructions
```

