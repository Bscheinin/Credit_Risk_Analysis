# Credit Risk Analysis
Credit risk arises from the chance that a borrower will be unable to meet their obligations to a lender. For banks, loans are the largest source of credit risk. 

## Overview of the Analysis
Determining credit risk can be done in many ways. This analysis uses machine learning to help determine credit risk for a lset of applicants from the LendingClub, a peer-to-peer lending service company. Credit risk is a crutial part of solvency for banks, therefore six different machine learning techniques were assessed to help determine credit risk for these applicants.

Each of the applicants were given a 'high_risk' or 'low_risk' score based on current loan performance. This metric was resampled in different ways in each of the techniques to determine if any of the machine learning models would accurately predict the risk score. The dataset had a large number of 'low_risk' applicants compared to the actual 'high_risk' applicants. This imbalance required application of different resampling techniques for prediction of credit risk.

## Results
The results for each of the six machine learning techniques are shown below. 

* **Naive Random Oversampling** duplicates the 'high_risk' scores in the training phase of the model in an attempt to balance the dataset. This methods accuracy score is 66%, the percision score shows a high false positive rate while the recall score of 60% means that nearly 40% of all actual 'high_risk' applicants were identified as such. 

<p align="center">
  <img width="600" height="300" src="https://github.com/Bscheinin/Credit_Risk_Analysis/blob/main/Images/Naive%20Over.PNG">
</p>

![Naive Random](https://github.com/Bscheinin/Credit_Risk_Analysis/blob/main/Images/Naive%20Over.PNG)

* **Synthetic Minority Oversampling Technique (SMOTE)** synthetically generates 'high_risk' scores to oversample the smaller samples during the training phase of the model in an attempt to balance the dataset. These results are very similiar to the Naive Random Oversampling results.

![SMOTE](https://github.com/Bscheinin/Credit_Risk_Analysis/blob/main/Images/SMOTE.PNG)

* **Undersampling** decreases the number of 'low_risk' scores in the training phase of the model through clustering these scores in an attempt to balance the dataset.

![UNDER](https://github.com/Bscheinin/Credit_Risk_Analysis/blob/main/Images/UNDER.PNG)

* **Combination Over and Under Sampling** works on both sample types; oversampling of the 'high_risk' score and undersampling the 'low_risk' scores during the training phase of the model in an attempt to balance the dataset and provide a higher rate of prediction. The accuracy score for this method is slightly lower than the previous models at 64%. The precision and recall scores are similiar.

![Combination](https://github.com/Bscheinin/Credit_Risk_Analysis/blob/main/Images/Combination.PNG)

* **Balanced Random Forest Classification** is one of the best ways to handle imbalanced data through classification of the credit scores. The accuracy score of this method is better than that of the sampling methods above at 78%. The precision score still shows a high number of false positive results but improved specificity scores.

![Forest](https://github.com/Bscheinin/Credit_Risk_Analysis/blob/main/Images/Random%20Forest.PNG)

* **Easy Ensemble Classification** creates multiple models and then combines them to improve prediction results. This method shows the best accuracy score at 92%. Additionally, the precision score shows the lowest number of false positive results and the greates recall scores.

![Easy](https://github.com/Bscheinin/Credit_Risk_Analysis/blob/main/Images/Ensemble.PNG)


## Summary
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.