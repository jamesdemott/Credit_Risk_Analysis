# Credit_Risk_Analysis

**Overview of the Analysis***
The purpose of my analysis was to examinea credit card dataset from LendingClub, clean and prepare this data set, and ultimately employ a variety of techniques to train and evaluate models with unbalanced classes. I employed resampling models to predict future credit risk using resampling, SMOTEEN, and ensemble classifiers. Below are my analysis of which models had high predictive capability. 

**Model Results**
##### Naive Random Oversampling:
* Balanced Accuracy Score: .637
* Precision:
  * High Risk: .01
  * Low Risk: 1.00
* Recall:
  * High Risk: .71
  * Low Risk: .56
##### SMOTE Oversampling:
* Balanced Accuracy Score: .654
* Precision:
  * High Risk: .01
  * Low Risk: 1.00
* Recall:
  * High Risk: .63
  * Low Risk: .68
##### Undersampling:
* Balanced Accuracy Score: .54
* Precision:
  * High Risk: .01
  * Low Risk: 1.00
* Recall:
  * High Risk: .68
  * Low Risk: .41
##### Combination Oversampling and Undersampling:
* Balanced Accuracy Score: .54
* Precision:
  * High Risk: .01
  * Low Risk: 1.00
* Recall:
  * High Risk: .72
  * Low Risk: .57
##### Balanced Random Forest Classifier:
* Balanced Accuracy Score: .974
* Precision:
  * High Risk: .09
  * Low Risk: 1.00
* Recall:
  * High Risk: .42
  * Low Risk: .98

##### Adaboost Classifier:
* Balanced Accuracy Score: .97
* Precision:
  * High Risk: .06
  * Low Risk: 1.00
* Recall:
  * High Risk: .85
  * Low Risk: .93

To summarize the results, I found that the ensemble classifiers tended to have far higher balanced accuracy scores. In the context of credit risk analysis, the priority should be to use a model which has a high sensitivity for the high risk groups so that LendingClub can deny these applications on the basis of high risk and avoid bad loans. 

Recall offers us a measure of the true positives which were correctly predicted. To this end, I recommend utilizing AdaBoost Classfier as this model has the highest recall score for high risk predictions, meaning that it is most likely to assist LendingClub in avoiding risky borrowers. 
