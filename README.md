# Credit_Risk_Analysis

## Overview
The purpose of this analysis is to predict credit risk given LendingClub data through the use of RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN, BalancedRandomForestClassifier, and EasyEnsembleClassifier.

## Results
### Oversampling
In the pursuit of this analysis, there were two methods of oversampling that were explored: RandomOverSampler and SMOTE.

- RandomOverSampler
- f1: 0.81
  - Accuracy: 0.646
  - Precision: 0.99
  - Recall: 0.68
![ROS](https://github.com/kramerkyle/Credit_Risk_Analysis/blob/main/Oversampling.png)

- SMOTE
-  f1: 0.77
  - Accuracy: 0.623
  - Precision: 0.99
  - Recall: 0.64
![SMOTE](https://github.com/kramerkyle/Credit_Risk_Analysis/blob/main/SMOTE.png)

### Undersampling
The first alternative of oversampling methods like ROS and SMOTE is Undersampling, especially through the ClusterCentroids method.

- ClusterCentroids
- f1 0.62
  - Accuracy: 0.529
  - Precision: 0.99
  - Recall: 0.45
![ClusterCentroids](https://github.com/kramerkyle/Credit_Risk_Analysis/blob/main/Undersampling.png)

### SMOTEENN
SMOTEENN is a combination of over and under-sampling that is also quite common.

- SMOTEENN
  - f1 0.7
  - Accuracy: 0.616
  - Precision: 0.99
  - Recall: 0.54
![SMOTEENN](https://github.com/kramerkyle/Credit_Risk_Analysis/blob/main/SMOTEENN.png)

### Bias Reduction
- BalancedRandomForestClassifier
  - f1 0.95
  - Accuracy: 0.925
  - Precision: 0.99
  - Recall: 0.91
![BRFC](https://github.com/kramerkyle/Credit_Risk_Analysis/blob/main/Balanced_RF.png)

- EasyEnsembleClassifier
  - f1 0.97
  - Accuracy: 0.925
  - Precision: 0.99
  - Recall: 0.94
![EEC](https://github.com/kramerkyle/Credit_Risk_Analysis/blob/main/EE_Classifier.png)

## Summary
These results look heartening. Many of the models expressed strong values across accuracy, precision, and recall. In this instance, oversampling yielded stronger models than undersampling and SMOTEENN.

All in all, the EasyEnsembleClassifier model has the strongest recommendation towards practical use due to it's high makrs across accuracy, precision, recall, and f1.
