# Credit Risk Analysis

## Overview of the Analysis
Using machine learning models, we ran a series of analysis to predict if a loan was a high or low credit risk. We were asked to use imbalanced-learn and scikit-learn libraries to create the machine learning models. We were provided with credit card data from LendingClub. With the various models created, we are trying to assess which of these would be best for predicting credit risk. 

## Results
### Oversampling
#### Naive Random Oversampling
![image1](https://github.com/DaniliukK95/credit_risk_analysis/blob/main/images/1.png)
- Accuracy: 65%
- Precision: High risk 1%, Low risk 100%, Average 99%
- Recall: High risk 60%, Low risk 69%, Average 69%
#### SMOTE Oversampling
![image2](https://github.com/DaniliukK95/credit_risk_analysis/blob/main/images/2.png)
- Accuracy: 62%
- Precision: High risk 1%, Low risk 100%, Average 99%
- Recall: High risk 60%, Low risk 64%, Average 64%

### Undersampling
#### Cluster Centroids
![image3](https://github.com/DaniliukK95/credit_risk_analysis/blob/main/images/3.png)
- Accuracy: 51%
- Precision: High risk 1%, Low risk 100%, Average 99%
- Recall: High risk 59%, Low risk 43%, Average 44%

### Combination (Over and Under) Sampling
#### SMOTEENN
![image4](https://github.com/DaniliukK95/credit_risk_analysis/blob/main/images/4.png)
- Accuracy: 64%
- Precision: High risk 1%, Low risk 100%, Average 99%
- Recall: High risk 70%, Low risk 57%, Average 57%

### Ensemble Learners
#### Balanced Random Forest Classifier
![image5](https://github.com/DaniliukK95/credit_risk_analysis/blob/main/images/5.png)
- Accuracy: 79%
- Precision: High risk 4%, Low risk 100%, Average 99%
- Recall: High risk 68%, Low risk 91%, Average 90%
#### Easy Ensemble AdaBoost Classifier
![image6](https://github.com/DaniliukK95/credit_risk_analysis/blob/main/images/6.png)
- Accuracy: 93%
- Precision: High risk 7%, Low risk 100%, Average 99%
- Recall: High risk 91%, Low risk 94%, Average 94%

## Summary
The model that provided the most useful results was the final model, the Easy Ensemble Classifier. This model had the best accuracy of all the models at 93%. This model also produced higher precision scores for the high risk at 7% which is important for the safety of banks. Finally, the recall score also proved to be well balanced and high with 91% for high risk and 94% for low risk. With this being said, the Easy Ensemble model is the best fit for predicting credit risk. 
