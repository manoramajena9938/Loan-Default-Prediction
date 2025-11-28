# Loan-Default-Prediction
Machine Learning model to predict loan defaults
**Loan Default Prediction — FinSecure (Machine Learning Project)**

This project builds a complete machine learning pipeline to predict whether a borrower will pay back a loan (1) or default (0) using historical loan application data from FinSecure, a peer-to-peer lending company.
The project includes EDA, preprocessing, model building, ROC-AUC evaluation, confusion matrix, and subgroup fairness analysis.

**Project Objective**
To develop a data-driven model that predicts the probability of loan repayment, allowing FinSecure to:
Reduce financial losses from loan defaults
Improve decision-making for loan approval
Ensure fairness across borrower subgroups

Target variable:
loan_paid_back = 1 → Loan fully paid
loan_paid_back = 0 → Loan defaulted

📂**Dataset Description**

The dataset includes borrower demographics, financial attributes, loan details, and repayment status.

Feature	Description
annual_income	Borrower's yearly income
debt_to_income_ratio	Debt ÷ Income
credit_score	Borrower's credit score
loan_amount	Amount requested
interest_rate	Assigned interest rate
gender	Male/Female
marital_status	Single / Married
education_level	High School, Graduate, etc.
employment_status	Employed / Unemployed
loan_purpose	Debt consolidation, home improvement, etc.
grade, subgrade	Risk indicators assigned by FinSecure
loan_paid_back	Target variable
**Project Workflow**
1️.Problem Formulation
Identify business need
Understand what loan default represents
2️.Exploratory Data Analysis

Includes:
Target distribution plot
Histograms of numeric features
Boxplots for outlier detection
Correlation heatmap

3️. Data Preprocessing
Using scikit-learn Pipeline + ColumnTransformer:
Missing value imputation
One-Hot Encoding for categorical features
Standardization for numeric features
Avoid data leakage

4️. Model Development
Models used:
Logistic Regression 
Hyperparameter tuning using GridSearchCV with ROC-AUC scoring.

5️.Model Evaluation
Metrics used:
ROC-AUC Score
ROC Curve
Confusion Matrix
Classification Report (Precision, Recall, F1)

6️.Subgroup Fairness Analysis
AUC evaluation across:
Different education levels
Top 3 and Bottom 3 loan purposes

 **Key Results**
Preprocessing pipeline worked effectively for mixed data types
Model achieved high ROC-AUC on test data
ROC Curve shows strong separation between positive and negative classes
Subgroup analysis shows variation across loan purposes but stable across education groups

Open the notebook
jupyter notebook notebooks/loan_default_pipeline.ipynb

Loan-Default-Prediction/
│
├── data/
│   └── loan_data.csv
│
├── notebooks/
│   └── loan_default_pipeline.ipynb
│
└── README.md

Author
Manorama Jena
B.Tech CSE,5th semester
FinSecure Loan Default Prediction Project


