# Credit Risk Analysis
## Overview of Project
The purpose of this project is to develop a Machine Learning Model to help predict high-risk loans. The following 6 supervised machine learning models will be used.
- Random Oversampling
- SMOTE Oversampling
- Undersampling
- Combination Sampling (Over and Under)
- Balanced Random Forest Classifier
- Easy Ensemble AdaBoost Classifier

To determine the effectiveness of each of these models, the precision and recall measures of these will be calculated and compared.

## Results

### Random Oversampling
![RandomOversampling](https://user-images.githubusercontent.com/67916327/187828925-463c67d9-e888-4032-9e5c-152e7f2ce1df.png)

- Accuracy Score: 0.65
- Precision: 0.01
- Recall:  0.62

### SMOTE Oversampling
![SMOTEOversampling](https://user-images.githubusercontent.com/67916327/187828967-3454cbce-11c1-4e62-992e-a358a3ba6edb.png)

- Accuracy Score: 0.63
- Precision: 0.01
- Recall: 0.62

### Undersampling
![Undersampling](https://user-images.githubusercontent.com/67916327/187828999-eb66d476-7beb-4a79-a489-b88b09912c6f.png)

- Accuracy Score: 0.59
- Precision: 0.01
- Recall: 0.61

### Combination Sampling (Over and Under)
![CombinationSampling](https://user-images.githubusercontent.com/67916327/187829022-027de906-4964-48f2-b4f6-10414b971013.png)

- Accuracy Score: 0.64
- Precision: 0.01
- Recall: 0.70

### Balanced Random Forest Classifier
![BalancedRandomForestClassifier](https://user-images.githubusercontent.com/67916327/187829048-92e88cbf-8616-4c27-ae78-83be139e0e66.png)

- Accuracy Score: 0.79
- Precision: 0.04
- Recall: 0.67

### Easy Ensemble AdaBoost Classifier
![EasyEnsembleAdaBoostClassifier](https://user-images.githubusercontent.com/67916327/187829058-3dadb79b-3180-4cfa-b48e-e8ee13b6f1bb.png)

- Accuracy Score: 0.92
- Precision: 0.07
- Recall: 0.90

## Summary
|                         | Random Oversampling | SMOTE Oversampling | Undersampling | Combination Sampling | Balanced Random  Forest Classifier | Easy Ensemble AdaBoost Classifier |
|-------------------------|---------------------|--------------------|---------------|----------------------|------------------------------------|-----------------------------------|
| Accuracy Score | 0.65                | 0.63               | 0.59          | 0.64                 | 0.79                               | 0.92                              |
| Precision               | 0.01                | 0.01               | 0.01          | 0.01                 | 0.04                               | 0.07                              |
| Recall                  | 0.62                | 0.62               | 0.61          | 0.70                 | 0.67                               | 0.90                              |

Given the performance of the models shown above, the Easy Ensemble AdaBoost Classifier Model performed the best in all the metrics. In the case of determining whether a loan is high-risk or low-risk, more importance should be given to the recall metric as it will determine the likelyhood of the model classifying a high-risk loan as high-risk. Given that the AdaBoost Model has the highest recall rate at 0.90, which is far ahead of the second best performing model (in terms of recall) at 0.70 in the combination sampling model.

Therefore, the AdaBoost Classifier Model should be used as it obtained the highest recall rate out of the 6 models.
