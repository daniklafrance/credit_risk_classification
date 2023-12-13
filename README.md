# credit_risk_classification

## Description

In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

## Getting Started

#### The instructions for this Challenge are divided into the following subsections:

* Split the Data into Training and Testing Sets
* Create a Logistic Regression Model with the Original Data
* Write a Credit Risk Analysis Report

## Setup

* numpy 1.21.6
* pandas 1.0.5
* scikit-learn 1.0.2
* imbalanced-learn 0.11.0

## Dependencies

* import numpy as np
* import pandas as pd
* from pathlib import Path
* from sklearn.metrics import balanced_accuracy_score, confusion_matrix, classification_report
* from imblearn.over_sampling import RandomOverSampler

## Grading

* Split the Data into Training and Testing Sets (30 points)
* Create a Logistic Regression Model (30 points)
* Write a Credit Risk Analysis Report (20 points)
* Coding Conventions and Formatting (10 points)
* Code Comments (10 points)

## Overview of the Analysis

The purpose of this analysis is to create a model that can accurately predict healthy loans and high-risk loans. 

The dataset was from over 75,000 loans. The information included the loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt and loan status.

Firstly, the y variable was set as the loan status column and the features were the all other columns.

Then the data was split into training and testing sets. I then created a logistic regression model, fit the model, made predictions using the test data and evaluated the performance.

Lastly, I repeated the above steps with resampled training data.

## Results


### Logistic Regression Model:

|            | precision | recall | f1-score | support |
|-----------:|:---------:|:------:|:--------:|:-------:|
| 0          |   1.00    |  0.99  |    1.00  |    18765|
| 1          |   0.85    |  0.91  |   0.88   |    619  |
|    accuracy|           |        |     0.99 |    19384|
|   macro avg|       0.92|    0.95|      0.94|    19384|
|weighted avg|       0.99|    0.99|      0.99|    19384|



### Logistic Regression Model with Resampled Training Data:

|            | precision | recall | f1-score | support |
|-----------:|:---------:|:------:|:--------:|:-------:|
| 0          |   1.00    |  0.99  |    1.00  |    18765|
| 1          |   0.84    |  0.99  |   0.91   |    619  |
|    accuracy|           |        |     0.99 |    19384|
|   macro avg|       0.92|    0.99|      0.95|    19384|
|weighted avg|       0.99|    0.99|      0.99|    19384|

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

## Authors

Danik Lafrance
[daniklafrance]([https://github.com/daniklafrance])

## References

Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.
