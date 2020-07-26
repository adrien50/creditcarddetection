# Credit Card Fraud Detection

## Project Introduction

It is often that the data we retrieve have imbalanced label and we are asked to make classification. These scenarios are troublesome since not only the models we usally use bring poor result, but also the evaluation metric we often used, accuracy, is not adequate for imbalanced data sets due to the impact of the minority class. This project aims to demonstrate some techniques used to combat these situations, such as resampling or cluster before predicting, as well as using PR (Precision-Recall) curve to evaluate model. The approaches for the project are :

Checking for missing values
Checking class imbalance
Distribution of variable ‘Time’ by class
Distribution of variable ‘Amount’ by class
Correlation of anonymised variables and ‘Amount’
Split data into train and test sets
create different versions of the training set as per sampling technique
apply various sampling techniques to the data and see the performance on the test set
test different models using the up sampling technique as that has given the highest auc score(logistic regression (GLM),logistic regression (GLM),random forest (RF))
With an auc score of 0.974 the XGBOOST model has performed the best 

Data Source: https://www.kaggle.com/mlg-ulb/creditcardfraud
It is a CSV file, contains 31 features, the last feature is used to classify the transaction whether it is a fraud or not.

# Information about data set

The datasets contains transactions made by credit cards in September 2013 by european cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues original features are not provided and more background information about the data is also not present. Features V1, V2, ... V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

Given the class imbalance ratio, we recommend measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC). Confusion matrix accuracy is not meaningful for unbalanced classification.







