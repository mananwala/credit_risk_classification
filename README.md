# Overview of the Analysis

## Purpose of this analysis

Credit risk poses a classification problem that’s inherently imbalanced. The reason is that healthy loans easily outnumber risky loans. The purpose of this analysis is to use various techniques to train and evaluate models with imbalanced classes.

## Financial information in the data and prediction

The dataset provided included the lending data. This dataset included the following information:

* Loan size
* Interest rate
* Borrower income
* Debt to income ratio
* Number of accounts
* Derogatory remarks
* Total debt
* Loan status

The purpose of this analysis is to predict the creditworthiness of borrowers.

The variables that I was trying to predict is loan_status.

## Steps

1. Resampled the dataset for model's accurate prediction
2. Defined the logical regression model to compare two versions of the dataset.  This was done using the imbalanced-learn library.
3. Subsequently, the RandomOverSampler module from the imbalanced-learn library is used to resample the data.
4. Finally, analyzed the count of the target classes,  calculated the balanced accuracy score, generated a confusion matrix, and a classification report.

## Results

* Machine Learning Model 1:
  *  Logistic Regression Model with the Original Data
        * Accuracy: 95.20%  
        * Precision: 85% 
        * Recall: 91%
<br></br>
* Machine Learning Model 2:
  * Logistic Regression Model with Resampled Training Data
    * Accuracy: 99%  
    * Precision: 84% 
    * Recall: 99%

## Summary

The accuracy achieved after resampling the data is much higher as compared to the original data. This is likely because of the higher accuracy score and recall score of the resampled data.

Predicting high-risk loan is more important as compared to healthy loan. As the recall score on the resampled data is higher, it can be concluded that the logistic regression model with resampled data has higher reliability.  