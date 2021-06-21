# Overview

Using a dataset from LendingClub, a peer-to-peer lending services company, the task required using undersampling the data with the ClusterCentroids algorithm and oversampling the data using RandomOverSample and SMOTE algorithms.  A combinatorial SMOTEENN algorithm was used for over and undersampling. To reduce bias, both BalancedRandomForestCalssifier and EasyEnsembleClassifier were utilized to predict credit risk.  This was done to better classify risky loans as good loans easily outnumber risky loans in an unblanaced blassification problem.

# Results

The balanced accuracy scores, precision and recall scores of all six machine learning results are as follows:

## Resampling

**Naive Random Oversampling**

* Balance Accuracy: 0.6495 
* High Risk Precision: 0.01 
* High Risk Recall: 0.73 
* Low Risk Precision: 1.00 
* Low Risk Recall: 0.57

![Naive Random Oversampling](https://user-images.githubusercontent.com/78942457/122699171-e3545380-d216-11eb-90a8-0db626b2183f.PNG)


**SMOTE Oversampling**

* Balance Accuracy: 0.6584
* High Risk Precision: 0.01
* High Risk Recall: 0.63
* Low Risk Precision: 1.00
* Low Risk Recall: 0.68

![SMOTE Oversampling](https://user-images.githubusercontent.com/78942457/122699178-e64f4400-d216-11eb-9885-b0e91e4c6206.PNG)


**Undersampling**

* Balance Accuracy: 0.6584
* High Risk Precision: 0.01
* High Risk Recall: 0.69
* Low Risk Precision: 1.00
* Low Risk Recall: 0.40

![Undersampling](https://user-images.githubusercontent.com/78942457/122699193-ef401580-d216-11eb-8f40-53abd126abef.PNG)


**Combination (Over and Under) Sampling**

* Balance Accuracy: .5442
* High Risk Precision: 0.01
* High Risk Recall: 0.78
* Low Risk Precision: 1.00
* Low Risk Recall: 0.54

![Combination](https://user-images.githubusercontent.com/78942457/122699201-f2d39c80-d216-11eb-8662-52e1c5baae55.PNG)


## Ensemble

**Balanced Random Forest Classifier**

* Balance Accuracy: 0.7885
* High Risk Precision: 0.03
* High Risk Recall: 0.70
* Low Risk Precision: 1.00
* Low Risk Recall: 0.87

![Balanced Random Forest Classifier](https://user-images.githubusercontent.com/78942457/122699210-f6672380-d216-11eb-84df-857c756eef30.PNG)


**Easy Ensemble AdaBoost Classifier**

* Balance Accuracy: 0.9317
* High Risk Precision: 0.09
* High Risk Recall: 0.92
* Low Risk Precision: 1.00
* Low Risk Recall: 0.94

![Easy Ensemble AdaBoost Classifier](https://user-images.githubusercontent.com/78942457/122699215-f9621400-d216-11eb-911c-3b94216763f3.PNG)


# Summary

None of the models that were used were particularly precise.  This could mean that the results would end up with high risk loans being missed.  Since the industry is already overwhelmed with low risk loans, and weeding out high risk loans is the objective I would not recommend any of these models.  While the Easy Ensemble offers the best results overall, a 93.2% Balance accuracy, and when it identifies a high risk loan, it will likely be correct with a sensitivity (recall) score of 0.92, it is just missing too many high risk loans.
