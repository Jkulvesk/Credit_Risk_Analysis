# Credit Risk Analysis

## Overview
The purpose of this analysis is to predict credit risk using six different models. The base data used in this analysis is a credit card credit dataset from LendingClub, a peer-to-peer lending services company. 
The target variable used in this analysis is the loan status - whether it is high or low risk. 

## Results
The results of the six machine learning models are below.
### Naive Random Oversampling
- Balanced Accuracy Score = 67.7%
- Precision Score = 1% (high risk); 100% (low risk); 99% (average)
- Recall Score = 76% (high risk); 59% (low risk); 59% (average)

### SMOTE Oversampling
- Balanced Accuracy Score = 66.2%
- Precision Score = 1% (high risk); 100% (low risk); 99% (average)
- Recall Score = 63% (high risk); 69% (low risk); 69% (average)

### Cluster Centroids Undersampling
- Balanced Accuracy Score = 66.2%
- Precision Score = 1% (high risk); 100% (low risk); 99% (average)
- Recall Score = 67% (high risk); 42% (low risk); 67% (average)

### SMOTEENN (over/under sampling combo)
- Balanced Accuracy Score = 54.4%
- Precision Score = 1% (high risk); 100% (low risk); 99% (average)
- Recall Score = 72% (high risk); 57% (low risk); 57% (average)

### Balanced Random Forest Classifier
- Balanced Accuracy Score = 75.5%
- Precision Score = 3% (high risk); 100% (low risk); 99% (average)
- Recall Score = 62% (high risk); 89% (low risk); 89% (average)
Most important features - see screenshot below.

![Screenshot](https://user-images.githubusercontent.com/72076683/107887289-a1af4700-6eca-11eb-8813-2f92e258f4ba.png)

### Easy Ensemble Classifier
- Balanced Accuracy Score = 93.2%
- Precision Score = 3% (high risk); 100% (low risk); 99% (average)
- Recall Score = 62% (high risk); 89% (low risk); 89% (average)

## Summary
In looking at all six models, there is not one that has high precision for predicting high risk loans. The best model is the Easy Ensemble Classifier which has the highest accuracy score and the highest sensitivity ratings. I would perform further analysis by only including variables like total received principle/interest/total payments and last payment amounts and total payment inv to further refine the model and determine the precision and sensitivity based on those factors alone. 

The analysis on its own, as is now, is not precise enought to predict high risk loans.
