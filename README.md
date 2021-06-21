# Overview

Using a dataset from LendingClub, a peer-to-peer lending services company, the task required using undersampling the data with the ClusterCentroids algorithm and oversampling the data using RandomOverSample and SMOTE algorithms.  A combinatorial SMOTEENN algorithm was used for over and undersampling. To reduce bias, both BalancedRandomForestCalssifier and EasyEnsembleClassifier were utilized to predict credit risk.  This was done to better classify risky loans as good loans easily outnumber risky loans in an unblanaced blassification problem.

# Results

The balanced accuracy scores, precision and recall scores of all six machine learning results are as follows:

## Resampling

**Naive Random Oversampling

* Balance Accuracy: 0.6495
* 
* High Risk Precision: .01
* 
* High Risk Recall: 0.73
* 
* Low Risk Precision: 1.00
* 
* Low Risk Recall: 0.57

**SMOTE Oversampling

* Balance Accuracy: 0.6584
* High Risk Precision: .01
* High Risk Recall: 0.63
* Low Risk Precision: 1.00
* Low Risk Recall: 0.68

**Undersampling

* Balance Accuracy: 
* High Risk Precision: 
* High Risk Recall: 
* Low Risk Precision: 
* Low Risk Recall: 

**Combination (Over and Under) Sampling

* Balance Accuracy: 
* High Risk Precision: 
* High Risk Recall: 
* Low Risk Precision: 
* Low Risk Recall: 

## Ensemble

**Balanced Random Forest Classifier

* Balance Accuracy: 
* High Risk Precision: 
* High Risk Recall: 
* Low Risk Precision: 
* Low Risk Recall: 

**Easy Ensemble AdaBoost Classifier

* Balance Accuracy: 
* High Risk Precision: 
* High Risk Recall: 
* Low Risk Precision: 
* Low Risk Recall: 

# Summary
