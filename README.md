# credit-risk-classification

## Report

### Overview of the Analysis

* Various techniques were used to train and evaluate a model based on loan risk. A dataset of historical lending activity from a peer-to-peer lending services company was used to build a model that can identify the creditworthiness of borrowers. 
* * I checked the balance of the loan_status to see the ratio of low risk to high risk loans. This was significant to note, as there were far more healthy loans than high-risk loans in the data set. 
* The data was then split into Training and Testing Sets and a Logistic Regression Model with the Original Data was created to predict the creditworthiness of borrowers.
* Then I calculated balanced accuracy score. created confusion matrix and ran a classification report.
* Then I resampled the data using RandomOverSampler. This increased the sample size for the high-risk loans to better predict them.

### Results

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  * Balanced accuracy = 95.2%
  * Precision for healthy loans = 100%
  * Precision for high-risk loans = 85%
  * Recall for healthy loans = 99%
  * Recall for high-risk loans = 91%
Machine Learning Model 1 does well on predicting healthy loans as the precision and recall are almost 100 percent. The model also has a high accuracy of 95%; however, in the context of this problem we want to make sure we predict risky loans with a higher degree of accuracy that is where the model is not performing as well as it should. The recall for risky-loans is only 91%.


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  * Balanced accuracy = 99.4%
  * Precision for healthy loans = 100%
  * Precision for high-risk loans = 84%
  * Recall for healthy loans = 99%
  * Recall for high-risk loans = 99%
In Machine Learning Model 2, the overall accuracy has increased from 95% to 99% and the recall for risky-loans has also increased from 91% to 99%. This model is better at predicting risky-loans as opposed to the previous model.

### Summary

* Machine Learning Model 1 does well on predicting healthy loans as the precision and recall are almost 100 percent. The model also has a high accuracy of 95%; however, in the context of this problem we want to make sure we predict risky loans with a higher degree of accuracy that is where the model is not performing as well as it should. The recall for risky-loans is only 91%.
* In Machine Learning Model 2, the overall accuracy has increased from 95% to 99% and the recall for risky-loans has also increased from 91% to 99%. This model is better at predicting risky-loans as opposed to the previous model.
* Performance depends on the problem we are trying to solve. For example, in this case it is more important to predict the 1's (high-risk loans) correctly as failing to do so could be very costly to the lender. In this case it would be better to use Machine Learning Model 2. 
