# Credit Risk Analysis
Credit risk arises from the chance that a borrower will be unable to meet their obligations to a lender. For banks, loans are the largest source of credit risk. 

## Overview of the Analysis
Determining credit risk can be done in many ways. This analysis uses machine learning to help determine credit risk for a lset of applicants from the LendingClub, a peer-to-peer lending service company. Credit risk is a crutial part of solvency for banks, therefore six different machine learning techniques were assessed to help determine credit risk for these applicants.

Each of the applicants were given a 'high_risk' or 'low_risk' score based on current loan performance. This metric was resampled in different ways in each of the techniques to determine if any of the machine learning models would accurately predict the risk score. The dataset had a large number of 'low_risk' applicants compared to the actual 'high_risk' applicants. This imbalance required application of different resampling techniques for prediction of credit risk.

## Results
The results for each of the six machine learning techniques are shown below. 

* Naive Random Oversampling duplicates the 'high_risk' scores in the training phase of the model in an attempt to balance the dataset.
![Deliverable 1 analysis](https://github.com/Bscheinin/MechaCar_Statistical_Analysis/blob/main/Deliverable%201%20analysis.PNG)

* Synthetic Minority Oversampling Technique (SMOTE) synthetically generates 'high_risk' scores to oversample the smaller samples during the training phase of the model in an attempt to balance the dataset.

* Undersampling decreases the number of 'low_risk' scores in the training phase of the model through clustering these scores in an attempt to balance the dataset.

* Combination Over and Under Sampling works on both sample types; oversampling of the 'high_risk' score and undersampling the 'low_risk' scores during the training phase of the model in an attempt to balance the dataset and provide a higher rate of prediction.

* Balanced Random Forest Classification is one of the best ways to handle imbalanced data through classification of the credit scores. 

* Easy Ensemble Classification creates multiple models and then combines them to improve prediction results.

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.