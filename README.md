# Credit_Risk_Analysis
# Overview
The purpose of this analysis is to predict credit risk (i.e find good candidates for credit cards) using Machine Learning algorithms based on different factors. The results from the different machine learning models were compared by calculating the balanced accuracy, precision and recall scores. Based on these calculations, the performance of these models were evaluated and a written recommendation was made on which model can be used to predit credit risk.
# Resources:
* Jupyter Notebook
* Libraries: pandas, Scikit-learn, pathlib
# Results
## Deliverable 1 & 2: Use Resampling Models to Predict Credit Risk
I used the following four models (i.e. Naive Random Oversampling, SMOTE Oversampling, Undersampling and Combination (Over and Under) Sampling) for both Deliverables 1 & 2 to predict credit risk.
###### Random Oversampling
The random oversampling model had the following metrics..
* Balanced Accuracy: 0.661
* Precision and Recall: This model predicted high risk datapoints with a precision of 0.01 and a recall of 0.72.

###### SMOTE Oversampling
The SMOTE oversampling model had the following metrics..
* Balanced Accuracy: 0.658
* Precision and Recall: This model predicted high risk datapoints with a precision of 0.01 and a recall of 0.62.

###### ClusterCentroids Undersampling
The ClusterCentroids Undersampling model had the following metrics..
* Balanced Accuracy: 0.658
* Precision and Recall: This model predicted high risk datapoints with a precision of 0.01 and a recall of 0.72.

###### Combination (Over and Under) Sampling
The Combination (Over and Under) Sampling model had the following metrics..
* Balanced Accuracy: 0.661
* Precision and Recall: This model predicted high risk datapoints with a precision of 0.01 and a recall of 0.77.

## Deliverable 3: Use Ensemble Classifiers Models to Predict Credit Risk
I used two Ensemble Classifiers Models (i.e. BalancedRandomForestClassifier and EasyEnsembleClassifier) for Deliverable 3 to predict credit risk.
###### Balanced Random Forest Classifier
The Balanced Random Forest Classifier model had the following metrics..
* Balanced Accuracy: 0.755
* Precision and Recall: This model predicted high risk datapoints with a precision of 0.03 and a recall of 0.62.

###### Easy Ensemble Classifier
The Easy Ensemble Classifier model had the following metrics..
* Balanced Accuracy: 0.932
* Precision and Recall: This model predicted high risk datapoints with a precision of 0.09 and a recall of 0.92.
# Summary
## Balanced Accuracy:
According to the models and the pictures above, the Easy Ensemble Classifier model had the highest balanced accuracy which is 93%; while both the SMOTE oversampling and ClusterCentroids Undersampling models have the lowest balanced accuracy at approximately 66%.  

## Precision:
According to the pictures above, all the models had a low precision for high risk applicants at < 10%. This shows that the different models assigned the high risk label to candidates that were not high risk.

## Recall:
According to the models and the pictures above, the Easy Ensemble Classifier model had the highest recall for high risk applicants which is 92%; while both the SMOTE oversampling and Balanced Random Forest Classifier models have the lowest balanced accuracy at approximately 62%. This shows that the Easy Ensemble Classifier model was good at detecting high risk applicants.

According to all the results above, I would recommend the Easy Ensemble Classifier model but with a little caution. This is due to the fact that it was able to detect high risk applicants and can be used to detct more high risk candidates.
