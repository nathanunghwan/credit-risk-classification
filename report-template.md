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
  * Description of Model 1 Accuracy, Precision, and Recall scores.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

Accuracy is 0.99, which is a very high accuracy. However, if the dataset is imbalanced, even high accuracy may not indicate good predictive power for the High-risk Loan
The precision of Healthy Loan and High-risk Loan are 1.00 and 0.85, respectively, indicating that there were more errors in predicting High-risk Loan.
The recall of Healthy Loan and High-risk Loan are 0.99 and 0.91, respectively. This means that there were cases where the model missed High-risk Loan, resulting in 56 False negatives.
Looking at the given results, the support for Healthy Loan (normal loans) is 18765, while that for High-risk Loan (risky loans) is 619. Therefore, the dataset is imbalanced, with Healthy Loan having significantly more data than High-risk Loan. As a result, the model shows very high precision and recall for Healthy Loan, but low precision and recall for High-risk Loan.
In particular, in the case of loans, predicting high-risk loans is important to prevent losses, so the recall value is crucial.


To solve the class imbalance problem, it is necessary to resample using an oversampling technique.
