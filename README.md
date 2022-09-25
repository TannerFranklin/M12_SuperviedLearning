# M12_SuperviedLearning

Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

The purpose of this analysis is to ass the credit worthiness of potential borrowers. In this analysis, we set out to evaluate whether to provide a loan to a customer based on the following criteria: Loan Size, Interest Rate, Borrower income, Debt to Income, Number of Accounts, Derogatory Marks and Total Debt. To analysis the credit worthiness the data was first split into a target variable and features for the classficiation model to be trained on. Next value counts were taken to look at the data, and split the data into feature training and testing data as well as target training and testing data. First step of the modeling process was to instantiate the logistic regression model and fit the model to training data using a random state parameter of 1. Once the data was fitted, the model was used to help predict the target value using the test features. After the model predictions were made the model performance was evaluated using the accuracy score, a confusion matrix, and classification report looking at the precision, recall, F1 Score and suppport metrics for each target variable.Once the first model and evaluation were compeleted, a second model was created using the oversampling method which helped in build another model to view our results.
Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

Machine Learning Model 1:

Description of Model 1 Accuracy, Precision, and Recall scores.

      precision    recall  f1-score   support

   0       1.00      0.99      1.00     18765
   1       0.85      0.91      0.88       619
accuracy 0.99 19384 macro avg 0.92 0.95 0.94 19384 weighted avg 0.99 0.99 0.99 19384

Machine Learning Model 2:

Description of Model 2 Accuracy, Precision, and Recall scores.

      precision    recall  f1-score   support

   0       1.00      0.99      1.00     18765
   1       0.84      0.99      0.91       619
accuracy 0.99 19384 macro avg 0.92 0.99 0.95 19384 weighted avg 0.99 0.99 0.99 19384

Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

It appears the Machine Learning Model 2 with over sampling works the best due to the improved F1 Score for predicted loans provided. The improved recall value from 0.91 to 0.99 is the driving factor for improved precision and recall in predicting successful loans. This improved F1 Score on High Risk loans allows for the lender to make better decisionsi in the face on uncertainty, and I would recommend the second model in predicting which loans to provide while considering that both models may be subject to slight overfitting.
