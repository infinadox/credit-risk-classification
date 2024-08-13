# Credit Risk Classification Report

## Overview of the Analysis

The purpose of this analysis is to evaluate the creditworthiness of borrowers using machine learning models, specifically a logistic regression model. The dataset used for this analysis contains historical lending information, where the primary objective is to predict whether a loan is likely to default (classified as `1`) or remain healthy (classified as `0`).

The key variable we aimed to predict is the `loan_status`, which indicates whether a loan is high-risk (`1`) or low-risk (`0`). In our dataset, the `loan_status` column had the following distribution:
- **Healthy Loans (`0`)**: 18,765 instances
- **High-Risk Loans (`1`)**: 619 instances

The machine learning process involved several stages:
1. **Data Preparation**: Splitting the dataset into features (`X`) and labels (`y`).
2. **Training and Testing Split**: Dividing the data into training and testing sets to evaluate the model’s performance.
3. **Model Selection**: Applying a logistic regression model (`LogisticRegression`) to the training data.
4. **Model Evaluation**: Assessing the model’s performance using accuracy, precision, and recall scores.

## Results

- **Logistic Regression Model**:
    - **Accuracy**: 0.99
    - **Precision**:
        - Healthy Loans (`0`): 1.00
        - High-Risk Loans (`1`): 0.85
    - **Recall**:
        - Healthy Loans (`0`): 0.99
        - High-Risk Loans (`1`): 0.91

## Summary

The logistic regression model demonstrated excellent performance, with an overall accuracy of 99%. It performed best in predicting healthy loans (`0`), with perfect precision and very high recall. For high-risk loans (`1`), the model also performed well, with a recall of 91%, indicating that it correctly identified the majority of loans that are at risk of defaulting.

Given these results, the logistic regression model is recommended for use, particularly in scenarios where it is crucial to accurately identify healthy loans and minimize false positives. However, if the primary concern is correctly identifying every high-risk loan (minimizing false negatives), further refinement or additional models may be necessary to improve the precision for high-risk loan predictions.

