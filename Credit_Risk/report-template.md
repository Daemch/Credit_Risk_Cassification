# Module 20 Credit Risk Analysis

## Overview of the Analysis

This analysis uses a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.
One technique, Logistic Regression was used to train and evaluate a model based on loan risk.
The steps taken in processing this data, as follows:

1. Split the data into training and testing Sets by creating the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
    In which, a value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.
2. Create a Logistic Regression Model and fit the training data (X_train and y_train), inorder to make predictions.
3. Maky predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.
4. Generate a confusion matrix and classification report.

## Results of confusion matrix and classification results

CLASSIFICATION MODEL

True negatives (0) are 14948. These are the number of samples correctly predicted as having a healthy loan status.

True positives (1) are 467. These are the number of samples correctly predicted as being at high-risk of defaulting.

False negatives are 33. These are the number of samples that were actually high-risk(1) but predicted as healthy(0).

False positives are 60. These are the number of samples that were actually healthy(0) but predicted to be high-risk(1).

ACCURACY SCORE

99.4% of the predictions were correct.

CLASSIFICATION REPORT

The precision ratio is the calculation of true positive predictions to the total predicted positives.

Healthy Loan Status(0) is 1.00, showing all predictions for 0 were correct.

High-risk Loan Status(1) is 0.89, showing that 89% if the predictions were actually class 1.


The recall ratio is the calculaion of true positive predictions to the total actual positives.

Healthy Loan Status(0) is 1.00, showing all predictions for 0 were correct.

High-risk Loan Status(1) is 0.93, showing that 93% if the predictions were actually class 1.


The F1-Score is the average between the precision and recall ratios.

Healthy Loan Status(0) is 1.00, showing a 100% balance of precision and recall for healthy loan status.

High-risk Loan Status(1) is 0.91, showing a great balance of precision and recall for high-risk loan status.


The support number is actual occurrences of each class in the dataset.

Healthy Loan Status(0) (15008): Majority class in the dataset.

High-risk Loan Status(1)(500): Minority class in the dataset.

Overall Performance:
Accuracy of 0.99, shows that the model performed very well.

Macro Avg of 0.95, is the average performance across both healthy and high=risk loans.

Weighted Avg of 0.99 is also another indicator of the average between healthy and high-risk loans.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?

The Logistic Regression Model provided demonstrates outstanding performance in all catagories.

Although, it is apparent that the report was suppose to include different models to compare and contrast. Due to increasing lack of continuity throughout this program, I can only recommend the Logistic Regression Model because that was the only model provided.

