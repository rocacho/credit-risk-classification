# credit-risk-classification
Module 20 Challenge
I solved this challenge leveraging the materials used in class

# Module 20 Report: Credit Risk Classification

## Overview of the Analysis
The main goal for this project was to use a machine learning model to evaluate and predict credit risk, by differentiating between healthy loans (identified wiht a 0) from high-risk loans (identified wiht a 1). For this we got to try with different machine learning models to have a comparisson of diferent scores and results that will allow us to identify the potentially best model for such a situation.

Th input data used was the one provided in the resources which has information about loans, such as: loan size,	interest rate,	borrower income,	debt to income,	num of accounts,	derogatory marks,	total debt and also we weer provided with a loan status taht used all this data to define if these loans ar higj risk or healthy.

The relevance of this project is that if we are able to hava a accurate model we will be ablo to predict the health of loans if we are able to put together data similar to the one provided. 

The original data was not balanced, We have 2,500 '0' (healthy loan) vs 75,036 '1' (high-risk loan)  which is 30 times more healthy loans compared to the high risk ones. To address this imbalance, we employed the RandomOverSampler technique to create a balanced training dataset using Logistic Regression model due to its simplicity and interpretability.

## Results

* Machine Learning Model 1 (Without Resampling):

Balanced Accuracy Score: 0.9924
Precision: '1' (high-risk loan) - 0.87 | '0' (healthy loan) - 1.00
Recall: '1' (high-risk loan) -  0.89 | '0' (healthy loan) - 1.00

We got a good accuracy score of 99.24%. We can observe  a good balance between precision and recall for high-risk loans, with a precision of 0.87 and a recall of 0.89. Whle healthy loans where perfectly balanced

* Machine Learning Model 2 (With RandomOverSampler):

Balanced Accuracy Score: 0.9952
Precision: '1' (high-risk loan) - 0.87 | '0' (healthy loan) - 1.00
Recall: '1' (high-risk loan) -  1.00 | '0' (healthy loan) - 1.00

For this model where we used the RandomOverSampler we outperformed the previous model, with a higher accuracy score of 99.52%. We also managed to maintain a the good  precision for high-risk loans at 0.87 but the interesting thing is that here we managed to get a  recall of 1.00. Given these we can assumet that with this approach we ar able to captures almost all actual high-risk loans.

## Summary
To be fair with both models we good pretty good numbers in terms of accuracy which let's us infeer that they are good for predicting credit risk. Also we could see numbers above 0.80 for Precision and Reacall, but here is hwere we can see superior results. This superiority alows us to have a more trustable model for identifying potential high-risk loans.

This alows us to demnstrate te importances of using balanced data and a suitable model for making accurate decisions, mostly whe we are talking about a delicate matter such as loans that can rpresent high impact on the financial health of an institution. 
