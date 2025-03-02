# Credit Risk Analysis Report

## Overview of the Analysis

* The purpose of this analysis is to evaluate the performance of a logistic regression model in predicting credit risk. The analysis aims to determine whether a loan is classified as healthy (0) or high-risk (1) based on financial data. The objective is to assess the accuracy, precision, and recall of the model to determine its suitability for making credit-related decisions.

## Data and Variables

The dataset consists of financial information related to loan applicants. The target variable is loan_status, where:

* 0 represents a healthy loan

* 1 represents a high-risk loan

* The features (X) include various financial attributes of the loan applicants, excluding loan_status. The distribution of the target variable is examined using value_counts() to understand the balance of the dataset.

## Machine Learning Process

The machine learning analysis follows these steps:

1. Data Preprocessing – Load and inspect the dataset, separate features and labels.

2. Train-Test Split – Split the dataset into training and testing sets.

3. Model Selection – Use Logistic Regression for classification.

4. Model Training – Train the model using the training dataset.

5. Model Evaluation – Assess the model using a confusion matrix, accuracy score, and classification report.

## Results

## Logistic Regression Model Performance:

* Accuracy Score: 99.25%

* Confusion Matrix:

    * True Positives (Healthy Loans correctly predicted): 18,658

    * False Positives (Healthy Loans misclassified as High-Risk): 103

    * False Negatives (High-Risk Loans misclassified as Healthy): 43

    * True Negatives (High-Risk Loans correctly predicted): 580

* Precision and Recall Scores:

* Healthy Loans (0):

    * Precision: 1.00

    * Recall: 0.99

* High-Risk Loans (1):

    * Precision: 0.85

    * Recall: 0.93

## Summary

The logistic regression model performed exceptionally well, achieving an overall accuracy of 99.25%. The model is highly effective in predicting healthy loans (0), with a precision of 1.00 and recall of 0.99. However, its performance on high-risk loans (1) is slightly lower, with 85% precision and 93% recall.

## Recommendation:

* If the goal is to minimize false positives (misclassifying healthy loans as high-risk), then this model is a strong candidate due to its near-perfect precision for 0.

* If the goal is to detect high-risk loans with higher accuracy, additional model tuning or alternative machine learning models (such as Random Forest or SMOTE-balanced Logistic Regression) may be needed.


