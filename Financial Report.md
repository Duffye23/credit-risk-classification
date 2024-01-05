# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

This challenge had the challenge of creating a supervised machine learning model to predict the health of a particular loan. The classification was broken down in to "healthy" loans, represented by a 0, and "high risk" loans, denoted by a 1. The model took into account a myriad of financial factors, included the size of the loan, the borrower's net income and debt to income ratio, and loan interest rate before giving us the variable that we would go on to predict: loan status. As stated, the purpose of this model was to predict the status of a loan, given the previously mentioned factors. This data included over 10000 rows, with a split of 75036 0 loans and 2500 1 loans. 

The machine learning model creation went as such:
1- Split the data into features(independent varaibles) and labels (the dependent variable)
2- Further split the data into training and testing data. This way I can train our model and then test its efficacy.
3- Select the type of machine learning model to use. In this case a Logistic Regression was used for its ability to predict label data.
4- The model was then fit and trained on the training data.
5- Once trained, the model was made to predict label outcomes on the test data.
6- Finally, the model was then evaulated based on its precision, recall, and accuracy.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  - Accuracy: 0.9520479254722232
  - Precision: 
    - 0: 1.00
    - 1: .85
  - Recall: 
    - 0: .99
    - 1: .91

## Summary

The model is near flawless in its precision with predicting 0 (healthy loans), however its precision in predicting 1 (high risk loans) is much lower. In general, the model's ability to properly receall and be precise is lower for the 1 designation in general. In conclusion, it is near flawless in its precision of 0 but leaves something to be desired with 1. If the goal is to correctly identify healthy loans, this model would be near perfect, as it's precision and recall for label 0 are 1.00 and .99 respectively. However, the model will need further tuning if it is to be used as a predictor for label 1. The numbers are simply below a threshold I would feel comfortable with trusting as .85 precision and .91 recall are less than ideal when providing loans.
