# Credit_Risk_Analysis

##Purpose

The purpose of this assignment was to determine the best machine learning models between "Balance Random Forest Classifier" and "Easy Ensemble Classifier" that redice bias to predict the credit risk. As such three different models were used to predict the risk as follows:
1) Resampling
2) SMOTEENN
3) Ensemble Classifiers.

##Results

Naive Random Oversampling

<img width="1127" alt="Screen Shot 2022-02-22 at 10 42 13 PM" src="https://user-images.githubusercontent.com/90429568/155258230-7f820655-e117-40d6-9028-03db253c2df3.png">

From this output it should be noted that the balanced accuracy score is 54%. Additionally, the high precision risk is about 1%, making f1 2% with imbalanced precison recall of 69%

Smote Oversampling

<img width="1440" alt="Screen Shot 2022-02-22 at 10 49 53 PM" src="https://user-images.githubusercontent.com/90429568/155258807-bfcf490c-2697-4d55-af3c-34b0ac8dadb8.png">

Smote oversampling results are similar to random oversampling, where balanced score is 62% and high precision risk is about 1% again. Imabalanced recall rate is 69%.

Cluster Centroids

<img width="1440" alt="Screen Shot 2022-02-22 at 10 53 29 PM" src="https://user-images.githubusercontent.com/90429568/155259097-3463dc0d-5c3e-4b75-8c0b-024ec46ab3ca.png">

In this analysis, balanced accuracy score is down to 52%, with 1% high risk precision score. Imbalanced recall score is 61%. This seems to produce results that are a little bit lower than both naive random oversampling and smote oversampling.

SMOTEENN Combination (over and under sampling)

<img width="1440" alt="Screen Shot 2022-02-22 at 10 57 24 PM" src="https://user-images.githubusercontent.com/90429568/155259428-e9ea835f-8643-42cf-81e9-244737bce6f7.png">

When both oversampling and under sampling are combined, balanced accuracy score is 65%. Precision high score is still the same, sitting at 1%. Specificity is 62% and recall is 69%. So far, this modelling method has the highest recall rate for imbalanced high_risk. 

Balanced random forest classifier

<img width="1440" alt="Screen Shot 2022-02-22 at 11 07 38 PM" src="https://user-images.githubusercontent.com/90429568/155260221-3b7a9e56-977a-4634-a13a-97ad298a6ef9.png">

Balanced accuracy score- 72%. High risk precision rate is 7%. High risk imbalanced recall 49%. 

<img width="1440" alt="Screen Shot 2022-02-22 at 11 09 57 PM" src="https://user-images.githubusercontent.com/90429568/155260428-67dc7c81-007e-4db9-b230-035cb2bccd04.png">

Easy Ensemble AdaBoost Classifier

Balanced accuracy score- 92%. High risk precision rate is 7%, high risk imabalanced recall is 94%. 

From these outputs, it can be safely established that both the Naive and Smote had similar results. SMOTEENN had further improvement, and forest classifier took a hit to the recall. As such, AdaBoost with both accuracy and recall over 90%.

**Summary

Since, the AdaBoost had the recall of 91%, indicating that this strategy predicted 91% of actual high risk loans. Additionally, all the other models showed poor precision rates, indicative of high false positives. An approach to address the number of false positives is still needed. 






