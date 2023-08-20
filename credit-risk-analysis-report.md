# Module 12 Credit Risk Analysis Report

## Overview of the Analysis

The objective of the analysis was to use machine learning models to predict the status of loans, determining whether they were considered "healthy" (0-label) or "high-risk" (1-label).  The data used to create the models had the following characteristics:

- loan size
- interest rate
- borrow income
- debt to income ratio
- number of accounts
- derogatory marks
- total debt
- loan status

During the process of the analysis, we pre-processed the data and split it up into training and testing sets.  Initially, we used a LosgisticRegression model on the test set, but when that did not yeild acceptable results, we used a resampling function to help balance out the data.

## Results

Machine Learning Model 1 (Original Logistic Regression):

Accuracy: Approximately 94%
Precision for label 0 (healthy loan): 97%
Recall for label 0 (healthy loan): 97%
Precision for label 1 (high-risk loan): 3%
Recall for label 1 (high-risk loan): 3%
Machine Learning Model 2 (Logistic Regression with Oversampling):

Accuracy: Approximately 99%
Precision for label 0 (healthy loan): 100%
Recall for label 0 (healthy loan): 99%
Precision for label 1 (high-risk loan): 84%
Recall for label 1 (high-risk loan): 99%

## Summary

The first model used only the logistic regression model and gave substantially acceptable results when predicting the healthy loans, but yeilded exceptionally poor results when predicting the high-risk loans.

The second model used the logistic regression model with oversampling and yielded even better results for healthy loans and an acceptably high percentage of high-risk loans.  While the high-risk loans started at about 3% before oversampling, they came up to mid 80s and even high 90 percentile. 

Given the success of the second model with oversampling, I would highly recommend that the institution uses it to in their application process.