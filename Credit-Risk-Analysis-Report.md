# Module 12 Report 

## Credit Risk Analysis Report

## Overview of the Analysis

* The purpose of the analysis is to compare the performance of 2 logistic regression machine learning models by evaluating loan risk that can be used to predict the creditworthiness of borrowers. Both models were used to predict the credit risk associated with financial loans.

* The objective of this analysis is to ultimately predict the status of the loan either as a '0'(healthy loan) or as a '1' (high-risk loan)


* The data was based on a dataset of financial information of historical lending activity from a peer-to-peer lending services company. Included in the dataset were the following categories: Loan Size,   Interest Rate, Borrower Income, Borrower Debt to Income Ratio , Borrower's Number of Credit Accounts, Derogatory Marks on the Borrower's Credit Report, Borrower's Total Debt and Borrower's Current Loan Status.  




* Describe the stages of the machine learning process you went through as part of this analysis.
*  The process I went through with this analysis was as follows:
1. Data Collection  - import the data containing relevant information to predict creditworthiness. 
2. Data Preprocessing- handling missing values, removing irrelevant features and formatting data into a suitable format for the testing and training. 
3. Feature Engineering - extracting relevant features from the datasetto make the predictions. 
4. Splitting the Data - dividing the preprocessed data into training and testing subsets.  The training set will be used to train the machine learning model, while the testing set will be used to evaluate its performance.
5. Model Selection and Training:  selecting the appropriate regression model and executing the query by training the model using the training dataset and tune the hyperparameters to optimize its performance.
6. Model Evaluation - assessing the performance of the trained model using the testing dataset to evaluate the model's ability to predict the borrower's risk rating, 1 or 0. 
7. Predictions - once the model is trained and validated it can be used to make predictions on new data. 



## Results

* Machine Learning Model 1: Logistic Regression on Original Data
* 
The accuracy for this model yielded and accuracy score of 99%, overall.  
The healthy loans group yielded perfect precision, recall and F1 sccres of 1.00.
The high-risk loans yielded the following scores:
  precision: 87%
  recall: 89%
  F1: 88%


* Machine Learning Model 2: Logistic Regression on Resampled data
* 
The accuracy score remained unchanged at 99%.
The scores for the healthy loans (group 0) remained quite good, each (precision, recall and F1) coming in at 99% - though, these scores did each drop from 100% from the scores of the original data. 
The scores for the high-risk (group 1) loans were much better with the resampled data in this model.  The precision, recall and F1 scores all jumped to 99%, which is: 
  12% better than the results for the original data in precision,
  10% better than the results for the original data in recall, and
  11% better than the results for the original data in in F1.  
  
## Summary

For this example, the Logistic Regression Model (2)  trained with resampled data fared better and should be considered a superior option than the Logistic Regression Model (1) that used the original data, especially when it comes to high-risk loans.  Since the purpose of this is to determine creditworthiness and try to accurately assess the lender's calculated risk(s) associated with high-risk loans, this is precisely the improvement that makes using the oversampled dataset so much better here. 

