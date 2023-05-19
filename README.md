# credit-risk-classification

## Overview of the Analysis

The purpose of this analysis is to evaluate the performance of machine learning models on credit risk data. The data contains records of loans with the target information being whether or not the loans were healty or high-risk, this is what the machine learning models are predicting.

The process involves loading the data from a CSV, splitting it into training and test data then fitting the training data into a Logistic Regression model which would then try and predict healthy or high-risk loans on the test data. The data contains low samples of high-risk loans so a second Logistic Regression model fitted with data resampled via Random Oversampling is used.

Accuracy scores and classification reports are used to compare the performance of the models.

## Results

* Machine Learning Model 1(Logistic Regression on Original Data)
  - Balanced accuracy score: 94.43%
  - Healthy Loan Precision: 100%, Healthy Loan Recall: 100%
  - High-Risk Loan Precision: 87%, High-Risk Loan Recall: 89%



* Machine Learning Model 2(Logistic Regression on Resampled Data):
  - Balanced accuracy score: 99.60%
  - Healthy Loan Precision: 100%, Healthy Loan Recall: 100%
  - High-Risk Loan Precision: 87%, High-Risk Loan Recall: 100%

## Summary

The results indicate the second model performs better as it has a higher balanced accuracy score and higher recall value for high-risk loans. It is more vital for the models to be able to predict high-risk loans, in particular false negatives need to be minimised as unidentified high-risk loans would lead to losses. The second model has a very low number of false negatives and should be the one to use.
