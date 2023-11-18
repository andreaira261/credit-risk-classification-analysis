# Module 12 Report

## Overview of the Analysis

The primary objective of this analysis was to develop machine learning models to predict loan risk based on financial data. 

The dataset contains financial attributes related to loan applicants, including loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. 

The goal is to use this information to predict and classify loans into two categories: Healthy Loans (Class 0) and High-Risk Loans (Class 1) based on their associated risk factors or repayment potential. 

The analysis began by collecting lending data from a CSV file, followed by dividing it into features and the target variable ('loan_status'). The data was split into training and testing sets for model training and evaluation. 

In the analysis, the scikit-learn library's LogisticRegression method was used for its suitability in binary classification tasks and was trained using the training dataset. Subsequently, predictions were made on the test data, and various metrics were computed to assess the model's performance. Additionally, the imbalanced-learn library's RandomOverSampler was implemented to tackle class imbalance. This technique addresses skewed class distributions, specifically in the context of high-risk loans, by generating synthetic samples to create a more balanced dataset for improved model training and performance in predicting high-risk loans accurately.

## Results

* Machine Learning Model 1:
  * Balanced Accuracy Score: 0.952
  * Precision (Class 0 - Healthy Loan): 1.00
  * Recall (Class 0 - Healthy Loan): 0.99
  * Precision (Class 1 - High-Risk Loan): 0.85
  * Recall (Class 1 - High-Risk Loan): 0.91



* Machine Learning Model 2:
  * Balanced Accuracy Score: 0.994
  * Precision (Class 0 - Healthy Loan): 1.00
  * Recall (Class 0 - Healthy Loan): 0.99
  * Precision (Class 1 - High-Risk Loan): 0.84
  * Recall (Class 1 - High-Risk Loan): 0.99

## Summary

Model 1 showcases exceptional performance in identifying healthy loans, maintaining high precision and recall. For high-risk loans, it displays a slightly lower precision but still maintains good recall. The balanced accuracy score indicates a strong overall ability to predict both classes.

Model 2 demonstrates excellent performance in identifying both healthy and high-risk loans. It maintains high precision and recall for healthy loans, similar to Model 1. For high-risk loans, it displays a marginally lower precision but still maintains exceptional recall. The higher balanced accuracy score indicates superior overall predictive capability for both classes compared to Model 1.

Considering the importance of correctly identifying high-risk loans while minimizing false alarms (misclassifying healthy loans as high-risk), Model 1 might be more suitable due to its higher precision (0.85) for high-risk loans (Class 1), compared to Model 2's precision (0.84) for the same class.

Though Model 2 has a slightly higher recall for Class 1, the higher precision of Model 1 for high-risk loans implies it might result in fewer false alarms (misclassifications of healthy loans as high-risk), which is crucial in financial contexts to avoid unnecessary risk assessments or actions on healthy loans.
