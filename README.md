# Credit_Risk_Analysis

## Overview of the loan prediction risk analysis:
### The purpose of this analysis is to use machine learning techniques to solve a credit card risk classification problem using the credit card credit dataset from LendingClub. We use various resampling methods such as RandomOverSampler, SMOTE, ClusterCentroids, and SMOTEENN, as well as ensemble classifiers such as BalancedRandomForestClassifier and EasyEnsembleClassifier to predict credit risk. By evaluating the performance of these models we can make a recommendation on which model should be used to predict credit risk.

## Results
### Balanced accuracy is the average of the recall obtained on each class, used to evaluate classification models with imbalanced classes. Precision is a measure of how accurate a model's positive predictions are and is calculated as the ratio of true positives to the sum of true positives and false positives. Recall is a measure of a model's completeness and is calculated as the ratio of true positives to the sum of true positives and false negatives. Listed below displays the balanced accuracy score, precision, and recall scores of all six machine learning models.

### Naive Random Oversampling 
* Balanced accuracy score is 0.6249984891886339
* For the "high_risk" class:
  - Precision = 0.01
  - Recall = 0.60
* For the "low_risk" class:
  - Precision = 1.00
  - Recall = 0.65

![Naive Random Oversampling ](https://user-images.githubusercontent.com/118647523/231824175-d0d7b1c5-5a45-4fb5-9806-cd54ae56eaf1.png)

### SMOTE Oversampling 
* Balanced accuracy score is 0.6512584051472337
* For the "high_risk" class:
  - Precision = 0.01
  - Recall = 0.64
* For the "low_risk" class:
  - Precision = 1.00
  - Recall = 0.66

![SMOTE Oversampling](https://user-images.githubusercontent.com/118647523/231824190-a6f4646f-e7ad-4f4d-aea0-1bed8ad54a37.png)

### Undersampling 
* Balanced accuracy score is 0.5103017191018931
* For the "high_risk" class:
  - Precision = 0.01
  - Recall = 0.59
* For the "low_risk" class:
  - Precision = 1.00
  - Recall = 0.43

![Undersampling](https://user-images.githubusercontent.com/118647523/231824211-fe1ed5d3-d171-4595-beba-a9355ecdae16.png)

### Combination Sampling 
* Balanced accuracy score is 0.6501283182453639
* For the "high_risk" class:
  - Precision = 0.01
  - Recall = 0.72
* For the "low_risk" class:
  - Precision = 1.00
  - Recall = 0.58

![Combination Sampling ](https://user-images.githubusercontent.com/118647523/231824231-29f5278b-8149-4dff-8098-2842c7d06403.png)

### Balanced Random Forest Classifier 
* Balanced accuracy score is 0.7877672625306695
* For the "high_risk" class:
  - Precision = 0.04
  - Recall = 0.67
* For the "low_risk" class:
  - Precision = 1.00
  - Recall = 0.91

![Balanced Random Forest Classifier](https://user-images.githubusercontent.com/118647523/231824246-47734594-44cb-4a57-875f-519bf86bd1b2.png)

### Easy Ensemble AdaBoost Classifier
* Balanced accuracy score is 0.925427358175101
* For the "high_risk" class:
  - Precision = 0.07
  - Recall = 0.91
* For the "low_risk" class:
  - Precision = 1.00
  - Recall = 0.94

![Easy Ensemble AdaBoost Classifier](https://user-images.githubusercontent.com/118647523/231835520-9fdf59df-6d9e-4017-92b7-c76fdc41c9ea.png)

## Summary:
### From all the models tested, the Easy Ensemble AdaBoost Classifier performed the best with the highest balanced accuracy score of 0.925 and the highest recall score for the high-risk class at 0.91. The precision score for the high-risk class was still low at 0.07, but this is likely due to the highly imbalanced nature of the dataset. It is recommend using the Easy Ensemble AdaBoost Classifier for this problem.

