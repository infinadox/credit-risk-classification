# Credit Risk Classification Report

## Overview of the Analysis
The purpose of this analysis is to evaluate the creditworthiness of borrowers using a logistic regression model. The model is trained on historical lending data to predict whether a loan is likely to default (high-risk) or remain healthy (low-risk). This analysis helps the lending services company make informed decisions regarding loan approvals.

## Results
- **Accuracy Score:** 0.99
- **Precision Score:**
  - Healthy Loans (`0`): 1.00
  - High-Risk Loans (`1`): 0.85
- **Recall Score:**
  - Healthy Loans (`0`): 0.99
  - High-Risk Loans (`1`): 0.91

## Summary
The logistic regression model performed exceptionally well with an overall accuracy of 99%. It demonstrates high precision and recall for predicting healthy loans, making it highly reliable in identifying non-defaulting loans. The model also shows good performance in identifying high-risk loans, with a recall of 91%, meaning it correctly identifies the majority of loans that are at risk of defaulting.

Given these results, the model is recommended for use by the company to assess borrower creditworthiness, particularly for identifying healthy loans. However, continued monitoring and potential refinements are suggested to further improve its precision in detecting high-risk loans.
