# Credit_Risk_Analysis
# Overview
The purpose of this analysis is to predict credit risk (i.e. find good candidates for credit cards) using Machine Learning algorithms based on different factors. The results from the different machine learning models were compared by calculating the balanced accuracy, precision and recall scores. Based on these calculations, the performance of these models were evaluated and a written recommendation was made on which model can be used to predit credit risk.
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

![Random oversampling 1](https://user-images.githubusercontent.com/104453593/188340895-f702c32c-649a-4e74-a1d7-295a1b146ebf.PNG)


###### SMOTE Oversampling
The SMOTE oversampling model had the following metrics..
* Balanced Accuracy: 0.658
* Precision and Recall: This model predicted high risk datapoints with a precision of 0.01 and a recall of 0.62.

![SMOTE Oversampling 1](https://user-images.githubusercontent.com/104453593/188340927-8a7a77dd-daa3-44bc-8647-89df08b36e8d.PNG)


###### ClusterCentroids Undersampling
The ClusterCentroids Undersampling model had the following metrics..
* Balanced Accuracy: 0.658
* Precision and Recall: This model predicted high risk datapoints with a precision of 0.01 and a recall of 0.72.

![Undersampling 1](https://user-images.githubusercontent.com/104453593/188340949-cc528015-60a0-4a59-bc28-c0b182b532fe.PNG)



###### Combination (Over and Under) Sampling
The Combination (Over and Under) Sampling model had the following metrics..
* Balanced Accuracy: 0.661
* Precision and Recall: This model predicted high risk datapoints with a precision of 0.01 and a recall of 0.77.

![combination sampling 1](https://user-images.githubusercontent.com/104453593/188340965-314be125-f212-4999-9cb1-8fbda9218005.PNG)



## Deliverable 3: Use Ensemble Classifiers Models to Predict Credit Risk
I used two Ensemble Classifiers Models (i.e. BalancedRandomForestClassifier and EasyEnsembleClassifier) for Deliverable 3 to predict credit risk.
###### Balanced Random Forest Classifier
The Balanced Random Forest Classifier model had the following metrics..
* Balanced Accuracy: 0.755
* Precision and Recall: This model predicted high risk datapoints with a precision of 0.03 and a recall of 0.62.

![balancedrandom forest classifier](https://user-images.githubusercontent.com/104453593/188340981-11954430-1b50-4e1b-a909-c9b77689268b.PNG)


###### Easy Ensemble Classifier
The Easy Ensemble Classifier model had the following metrics..
* Balanced Accuracy: 0.932
* Precision and Recall: This model predicted high risk datapoints with a precision of 0.09 and a recall of 0.92.

![easy emsemble classifier](https://user-images.githubusercontent.com/104453593/188341002-45c2c815-25b8-42db-90e1-d8a9fe3816ac.PNG)


# Summary
## Balanced Accuracy:
According to the models and the pictures above, the Easy Ensemble Classifier model had the highest balanced accuracy which is 93%; while both the SMOTE oversampling and ClusterCentroids Undersampling models have the lowest balanced accuracy at approximately 66%.  

## Precision:
According to the pictures above, all the models had a low precision for high risk applicants at < 10%. This shows that the different models assigned the high risk label to candidates that were not high risk.

## Recall:
According to the models and the pictures above, the Easy Ensemble Classifier model had the highest recall for high risk applicants which is 92%; while both the SMOTE oversampling and Balanced Random Forest Classifier models have the lowest balanced accuracy at approximately 62%. This shows that the Easy Ensemble Classifier model was good at detecting high risk applicants.

According to all the results above, I would recommend the Easy Ensemble Classifier model but with a little caution. This is due to the fact that it was able to detect high risk applicants and can be used to detct more high risk candidates.
