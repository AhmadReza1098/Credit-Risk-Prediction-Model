## Dataset Description
This project’s dataset provides detailed information on each loan applicant and their borrowing request, supporting data-driven credit risk assessment and machine learning. Each record contains the following characteristics:

**person_age**: Represents the applicant’s age in years.

**person_income**: The applicant’s reported annual income, given in USD.

**person_home_ownership**: Type of home ownership, categorized as RENT, MORTGAGE, OWN, or OTHER.

**person_emp_length**: Length of employment for the applicant, measured in years.

**loan_intent**: Describes the principal reason for the loan, such as EDUCATION, MEDICAL, HOMEIMPROVEMENT, DEBTCONSOLIDATION, PERSONAL, or VENTURE.

**loan_grade**: A credit grade (e.g., A, B, C, D) assigned to the loan, reflecting the applicant’s perceived credit risk.

**loan_amnt**: The amount of loan requested or granted, in USD.

**loan_int_rate**: The interest rate applied to the loan, expressed as a percentage.

**loan_status**: The target label: 1 if the applicant defaulted on the loan, 0 if not.

**loan_percent_income**: The fraction of income the loan payment represents (loan amount divided by annual income).

**cb_person_default_on_file**: Indicates whether there is evidence of prior default in credit bureau records (Y for yes, N for no).

**cb_person_cred_hist_length**: The applicant’s credit history length in years.

Together, these features capture a holistic view of individual risk factors and credit behavior, enabling the development and evaluation of robust predictive models for loan default

# Credit-Risk-Prediction-Model

This project implements and compares machine learning models to predict credit risk (likelihood of loan default) using a real-world dataset. The goal is to provide reliable prediction tools for lenders to identify high-risk borrowers effectively.

## Dataset

- The dataset consists of features including borrower's age, income, home ownership, employment length, loan intent, loan amount, interest rate, credit history details, and loan status (default or not).
- Data cleaning, preprocessing, and feature engineering were performed to prepare the data for modeling.

## Models Implemented

1. **Logistic Regression**
   - A baseline model providing interpretable coefficients.
   - Achieved balanced performance with accuracy ~78%, F1 score ~78%.

2. **Random Forest Classifier**
   - An ensemble tree-based model improving classification accuracy.
   - Achieved accuracy ~94%, precision ~97%, recall ~91%, ROC-AUC ~98.5%.

3. **XGBoost Classifier**
   - Advanced gradient boosting algorithm with optimized performance.
   - Achieved accuracy ~95%, precision ~98%, recall ~91%, ROC-AUC ~98.4%.

## Evaluation Metrics

Key metrics used to evaluate model performance:
- **Accuracy:** Overall correctness of the model.
- **Precision:** Correct positive predictions among all positive predictions.
- **Recall:** Correct positive predictions among all actual positives.
- **F1 Score:** Harmonic mean of precision and recall.
- **ROC-AUC:** Ability to distinguish between classes.

## Usage

1. Clone the repository.
2. Install required libraries: pandas, numpy, scikit-learn, xgboost, imblearn, matplotlib, seaborn.
3. Load and preprocess the dataset.
4. Train the models and evaluate using test data.
5. Use the trained model to predict credit risk for new loan applicants.

## Results Summary

| Model             | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|-------------------|----------|-----------|--------|----------|---------|
| Logistic Regression| 78%      | 78%       | 78%    | 78%      | 86%     |
| Random Forest     | 94%      | 97%       | 91%    | 94%      | 98.5%   |
| XGBoost           | 95%      | 98%       | 91%    | 95%      | 98.4%   |


## Dashboard Overview
The Power BI dashboard in this project enables effective monitoring and comparison of three credit risk classification models: **XGBoost (XGB)**, **Random Forest (RF)**, and **Logistic Regression (LOGIT)**. Users can interactively explore performance metrics such as accuracy, precision, recall, and F1 score for both loan default and non-default outcomes, making it simple to compare and interpret the effectiveness of each approach.

Interactive visuals within the dashboard illustrate how features like home **ownership**, **income**, and **debt-to-income** ratio relate to both model predictions and actual loan outcomes. These comparisons help stakeholders understand the strengths and weaknesses of each model and make informed decisions about credit risk strategies. Among the evaluated algorithms, XGBoost demonstrates the highest predictive performance, followed by Random Forest and Logistic Regression, as clearly reflected in the dashboard’s summary statistics and visual reports.
