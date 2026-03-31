# Loan_Approval_Prediction_SVM
A machine learning project that builds a Support Vector Machine (SVM) model to predict loan approval status based on various applicant features such as gender, marital status, education, income, credit history, and property area. The project involves data preprocessing, exploratory data analysis, model training, and evaluation.

# Loan Approval Prediction using Support Vector Machine (SVM)

## Overview
This project aims to develop a machine learning model to predict whether a loan application will be approved or rejected. By analyzing various applicant details, the model assists financial institutions in making informed decisions, reducing risk, and streamlining the loan application process. The core of this project is a Support Vector Machine (SVM) classifier.

## Features
- **Data Preprocessing**: Handles missing values, encodes categorical features, and transforms data for model compatibility.
- **Exploratory Data Analysis (EDA)**: Visualizes key relationships between features and the loan approval status.
- **SVM Classifier**: Implements a Support Vector Machine model for binary classification (Loan Approved/Rejected).
- **Model Evaluation**: Assesses the model's performance using metrics like accuracy score.

## Dataset
Dataset Link: "https://www.kaggle.com/datasets/ninzaami/loan-predication"
The dataset used in this project contains historical information about loan applicants, including:
- `Loan_ID`: Unique loan identification
- `Gender`: Male/Female
- `Married`: Yes/No
- `Dependents`: Number of dependents
- `Education`: Graduate/Not Graduate
- `Self_Employed`: Yes/No
- `ApplicantIncome`: Applicant's income
- `CoapplicantIncome`: Co-applicant's income
- `LoanAmount`: Loan amount requested
- `Loan_Amount_Term`: Term of loan in months
- `Credit_History`: Credit history meets guidelines (1.0/0.0)
- `Property_Area`: Urban/Semiurban/Rural
- `Loan_Status`: Loan approved (Y/N) - **Target Variable**

## Methodology
1.  **Data Loading**: The dataset is loaded using pandas.
2.  **Data Cleaning**: Missing values are handled by dropping rows with `NaN` values, and the `Dependents` column's '3+' category is converted to '4'.
3.  **Feature Engineering**: Categorical features like 'Gender', 'Married', 'Education', 'Self_Employed', and 'Property_Area' are converted into numerical representations using label encoding.
4.  **Data Splitting**: The dataset is divided into training and testing sets (e.g., 90% training, 10% testing).

## Results
The SVM model achieved an accuracy of approximately 79.86% on the training data and 83.33% on the test data. This indicates a good generalization capability of the model in predicting loan approval.
6.  **Model Training**: A Support Vector Machine (SVM) classifier with a linear kernel is trained on the preprocessed training data.
7.  **Model Evaluation**: The trained model's performance is evaluated on both training and test datasets using accuracy scores.
