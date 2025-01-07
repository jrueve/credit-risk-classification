# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
To use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

* Explain what financial information the data was on, and what you needed to predict.
Financial information found on text file named lending_data.csv which had columns: loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, total_debt, and loan_status. Data was on low or high risk loan status provided by lending company. Use of the Logistic Regression Algorithm was used in the machine learning model, because it is a tool used to predict probability of variable we are intersted in.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
The varible of interest was loan risk low(healthy) or high(un-healthy).

* Describe the stages of the machine learning process you went through as part of this analysis.
Construction of a logistic regression model, first by splitting the data into training and testing sets to compare the model after training. The model was fit to the training data and then the model was used to predict based on the test data.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).
Logistic Regression finds relationship between two factors and predicts the value of one based on another. The test_train-split is used to split the data into that which will train the model and that which we will use to test it's accuracy in prediction. Then we set up a confucion matrix to see if it predicts negative and if the value is actually negative. The same for positive. This gives shows amount of times in numbers the model is correct or incorrect in preediction.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
Based on the recall scores from the model the predictions made a mistake of around 1% for healthy loans and 6% for unhealthy loans. The accuracy score genrerated was 97%.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

The model trained on imbalanced data was the only model given in the homework files. It showed an accuracy of 97% which is a high degree of accuracy for prediction models. That said if the model was trained on oversimplified data instead of unbalanced data then I believe that model would provide a higher accuracy score than what was scored above. If we are trying to minimize risk then predicting the 1's are more important than the 0's, but if we are trying to evaluate whether the borrowers are not risky, or in other words if we are trying to expand lending services to as many low risk borrowers, then the 0's are more imporant.
