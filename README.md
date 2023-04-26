# credit-risk-classification

## Overview of the Analysis

The objective of this analysis is to assess the efficacy of two logistic regression machine learning models in forecasting the credit risk associated with loans. The study utilizes financial information, with particular emphasis on features such as loan amount, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The purpose is to predict the loan's status, which can either be considered a healthy loan (0) or a high-risk loan (1).

This analysis follows a machine learning process that includes the following stages:

* Data splitting: The data is split into training and testing datasets.
* Model creation: A logistic regression model is created and fitted with the training data.
* Prediction: The fitted model is used to make predictions using the test data. 
* Model evaluation: The model's performance is evaluated using accuracy and precision by comparing predicted and y test values.
* Data resampling: RandomOverSampler is used to resample the data to address class imbalance.
* Model Re-evaluation: The model is fit with the resampled data and predictions are made. Performance is re-evaluated. 

## Results

* Machine Learning Model 1:
  * The logistic regression model performed well in predicting healthy and high-risk labels, as indicated by the classification report. Both classes achieved high precision and recall. For the healthy loan class, a precision of 1.00 and recall of 0.99 were achieved, while the high-risk loan class obtained a precision of 0.85 and recall of 0.91. Overall, the model achieved an accuracy of 0.99, indicating strong performance in predicting both healthy and high-risk loans.


* Machine Learning Model 2:
  * The logistic regression model performed well in predicting healthy and high-risk labels, as indicated by the classification report. Both classes achieved high precision and recall. For the healthy loan class, a precision of 1.00 and recall of 0.99 were achieved, while the high-risk loan class obtained a precision of 0.84 and recall of 0.99. Overall, the model achieved an accuracy of 0.99, indicating strong performance in predicting both healthy and high-risk loans.
  
## Summary

Both models predict nearly identically. The purpose of these models are to predict if a loan is healthy or high risk. It is more important to predict the high risk loans than the healthy ones. If the cost of false positives is relatively low, then the oversampled model with higher recall (0.99) may be preferred as it can accurately capture almost all high risk loans. However, if the cost of false positives is high, then the initial model with a higher precision (0.85) may be preferred as it minimizes the number of false positives while still maintaining a relatively high recall.