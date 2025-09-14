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
