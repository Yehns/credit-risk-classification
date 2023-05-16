# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:

  * First splits the data into training and testing sets.
  * Data indicates a greater count of 0 values (low-risk loans)
  * The model uses a LogisticRegression fit for the x and y training values
  * The balanced accuracy score was 0.9218
  * The confusion matrix had TP count of 18663, and TN count of 563
  * The f1-scores in the classifcation report were 1.00 for 0 values and 0.88 for 1 values
  * This method had a high balanced accuracy score, but lacked in the accuracy for 1 values as the lassifcation report yielded low values. May be due to the spread/imbalance of data



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  * Second method utilised the RandomOverSampling, which randomly removes data from the training dataset
  * Uses a random_state of 1, which could be increased for further testing
  * The balanced accuracy score was 0.9936
  * The confusion matrix had a TP count of 18649 and a TN count of 615, greater than that of method 1
  * The f1 scores in the classification report were 1.00 for 0 values and 0.91 for 1 values
  * The repcision scores were lower than that of method 1 with 1.00 for 0 values and 0.84 for 1 values
  * As the f1-score is a weighted average of the repcision and recall, the second method suggests greater accuracy

## Summary

Summarise the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? ) 
It appears using machine learning in this scenario is context based. As the data focuses on low (0) vs high (1) risk bank loans, situatioanlly there should be a greater accuracy to high-risk loans. Comparing the two machine learning models, model 2 presents greater results and accuracy and thus should be preferred over the first method. Although, it shuold be further trained to reach a greater f1-score of 1 in the classification report. 

If you do not recommend any of the models, please justify your reasoning.
