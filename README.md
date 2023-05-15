# credit-risk-classification
Supervised Machine Learning 

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

We use various techniques to train and evaluate a model based on loan risk. 
This is based on a dataset of historical lending activity from a peer-to-peer lending services company.
Goal is to build a model that can identify the creditworthiness of borrowers.
The dataset is imabalanced where 96% of the dataset is `0` (healthy loan) and  4% fall into the `1` (high-risk loan) labels.

Steps followed -
Split the Data into Training and Testing Sets
Create a Logistic Regression Model with the Original Data - Training Data
Save the predictions on the testing data labels by using the testing feature data (X_test) and the fitted model
Evaluate the model’s performance by doing the following: Calculate the accuracy score of the model,Generate a confusion matrix and 
print the classification report.
Next use the RandomOverSampler module from the imbalanced-learn library to resample the data. Be sure to confirm that the labels have an equal number of data points.
Use the LogisticRegression classifier and the resampled data to fit the model and make predictions.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  
A balanced score of 0.9520479254722232 indicates that the model has a high average recall across all classes, suggesting that it is able to predict both the both the `0` (healthy loan) and `1` (high-risk loan) labels accurately.

Precision: Precision measures the proportion of positive predictions that were correct. In this case, for class 0, the precision is 1.00, which means that all of the samples predicted as 0 were actually 0. For class 1, the precision is 0.85, which means that 85% of the samples predicted as 1 were actually 1.

Recall: Recall measures the proportion of actual positive samples that were correctly predicted. In this case, for class 0, the recall is 0.99, which means that 99% of the actual 0 samples were correctly predicted as 0. For class 1, the recall is 0.91, which means that 91% of the actual 1 samples were correctly predicted as 1.

F1-score: F1-score is the harmonic mean of precision and recall. It provides a single score that balances both precision and recall. In this case, for class 0, the F1-score is 1.00, which indicates that the model is performing well for class 0. For class 1, the F1-score is 0.88, which indicates that there is some room for improvement in the model's performance for class 1.

Overall, the classification report indicates that the model is performing well for class 0 with high precision, recall, and F1-score. However, the model's performance for class 1 is not as good, with lower precision, recall, and F1-score.


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

A balanced accuracy score of 0.9936781215845847 indicates that the model has a very high average sensitivity (recall) across all classes, suggesting that it is able to predict both the majority and minority classes accurately

Precision: For class 0, the precision is 1.00, which means that all of the samples predicted as 0 were actually 0. For class 1, the precision is 0.84, which means that 84% of the samples predicted as 1 were actually 1.

Recall: Recall measures the proportion of actual positive samples that were correctly predicted. In this case, for class 0, the recall is 0.99, which means that 99% of the actual 0 samples were correctly predicted as 0. For class 1, the recall is 0.99, which means that 99% of the actual 1 samples were correctly predicted as 1.

F1-score: F1-score is the harmonic mean of precision and recall. It provides a single score that balances both precision and recall. In this case, for class 0, the F1-score is 1.00, which indicates that the model is performing well for class 0. For class 1, the F1-score is 0.91, which indicates that there is some room for improvement in the model's performance for class 1.

Overall, the classification report indicates that the model is performing well for both classes with high precision, recall, and F1-score. However, the model's performance for class 1 is slightly lower than that for class 0, with a lower precision and F1-score.
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )



If you do not recommend any of the models, please justify your reasoning.



