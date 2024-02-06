# credit-risk-classification
#Challenge Assignment 20 - Supervised Learning Report Template

## Overview of the Analysis

* The purpose of this analysis is to determine loan risk based on historical lending activity.
* The financial information includes loan size, interest rates, borrower incomes, debt to income ratios, # of accounts, derogatory marks, and total debt. We are trying to determine if a loan is healthy or has high-risk.
* We are trying to predict `loan_status` - `0` is a healthy loan, and `1` is a high-risk loan.
* We first split the data into testing and training data with sklearn (`train_test_split`). Then after creating a model, we made predictions, and evaluated model performance with a confusion matrx and classification report.
* Logistic Regression was used to create a model with the original data. 

## Results



* Logistic Regression Model:
  * The logistic regression model predicts the `0` healthy loan almost perfectly. The precision indicates all loans predicted as healthy are in fact healthy (`1.0` precision), and the `0.99` recall shows that almost all healthy loans are being found. The `1` high-risk loans still did fairly well with a precision of `.85` and a recall of `.91`, but not as accurate or complete as the healthy loans.

## Final Thoughts

* The model seemed to be performing relatively well with a very high overall accuracy score and it does a great job identifying nearly all healthy loans out there as well as doing that precisely. 
* I would definitely prefer that it did better at identifying higher risk loans (`1`). It didn't do an awful job but I would want it to be identifying as many of these as possible (recall). It should be fairly precise as well to not flag too many healthy loans as high-risk. 

