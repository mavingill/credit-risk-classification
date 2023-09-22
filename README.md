# credit-risk-classification



Write-Up Report:

# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).


Answer 1:
The purpose of this analysis was to take historical data of peer-to-peer loans and determine the creditworthiness of borrowers.
The financial information the data was on loan amounts, borrower incomes, interest rates, total loan amounts and more data. We needed to predict those total amounts of borrowers. We used 'value_counts' to generate this loan balance amount and then split the data into training and testing datasets. 
The stages we went through overall were to read in the data and create dataframes, filter the dataset by variables, split the overall dataset into training and testing datasets, use logistic regressions to analyze those subsequent datasets, and then come to conclusions about the accuracy and precision of the analysis. 




## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
    
  * Accurary Score: 0.94426
  * Precision of '0' (healthy loan): 1.00
  * Precision of '1' (high-risk loan): 0.87
  * Recall of '0': 1.00
  * Recall of '1': 0.89
  * F1 of '0': 1.00
  * F1 of '1': 0.88



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
    
  * Accuracy Score: 0.99597
  * Precision of '0': 1.00
  * Precision of '1': 0.87
  * Recall of '0': 1.00
  * Recall of '1': 1.00
  * F1 of '0': 1.00
  * F1 of '1': 0.93
 







## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.


Overall, the results indicated that in the first model, the '0' category (healthly loan) was a good predictive measure of the true score, however it was not for the '1' category (high-risk loan). 
Conversely, the 2nd model was a good predictive measure of the true score for '0', but was better overall for the '1' category. 
We know that these models perform better than the others in their respective ways by analyzing their accuracy, precision and recall scores. We can gather that since Model 1 was better overall for healthy loans, then we can use this model when looking at predictions for healthy loans. Alternatively, we can use Model 2 to make predictions on the high-risk loans, so the best use for each model would be to use them when analzying a specific type of loan. 




