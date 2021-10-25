# Credit Risk Analysis

## Overview of the Project
Assessing credit risk is an important endeavour conducted by orgnaizations before issuing loans to their applicants. The applicant must be evaluated over many different criteria to ensure that they have the ability to pay back the loan in the future. Because of the huge amount of data involved in this process, it is useful to use machine learning models to learn from pre-existing data and develop algorithms that can be applied to future loan applications. As such, this project uses a variety of models from the imbalanced-learn and scikit-learn libraries to conduct resampling and assess credit risk.

## Results

Six machine learning models were used in this analysis, with an evaluation of each below:

### ___Naive Random Oversampling___

<img width="583" alt="Screen Shot 2021-10-24 at 4 10 08 PM" src="https://user-images.githubusercontent.com/84816495/138611012-f06a982b-8163-414e-be11-c2634b889eb9.png">
<img width="714" alt="Screen Shot 2021-10-24 at 10 08 39 PM" src="https://user-images.githubusercontent.com/84816495/138624223-c91e04eb-2adf-45f2-818c-d8f9c688f94c.png">


As seen from above, the balanced accuracy score is 65.5% for this model.
For high_risk, the precision is only 1% while the sensitivity (recall) is 70%. The F1 score is therefore 0.02. For low_risk, the precision is 100% while the sensitivity (recall) is 61%. The F1 score is therefore 0.76.


### ___Oversampling with SMOTE___

<img width="371" alt="Screen Shot 2021-10-24 at 9 54 52 PM" src="https://user-images.githubusercontent.com/84816495/138623249-8387baa6-08d3-4aee-bb05-8f1a45259e91.png">
<img width="708" alt="Screen Shot 2021-10-24 at 10 09 26 PM" src="https://user-images.githubusercontent.com/84816495/138624274-85998b49-f530-4e0f-a597-423f03092013.png">


As seen from above, the balanced accuracy score is 66.2% for this model.
For high_risk, the precision is 9% while the sensitivity (recall) is 63%. The F1 score is therefore 0.16. For low_risk, the precision is 100% while the sensitivity (recall) is 69%. The F1 score is therefore 0.82.


### ___Undersampling with Cluster Centroids___

<img width="450" alt="Screen Shot 2021-10-24 at 9 58 04 PM" src="https://user-images.githubusercontent.com/84816495/138623462-42ef2523-9fb9-4f1e-bd26-849814d2a3f1.png">
<img width="709" alt="Screen Shot 2021-10-24 at 10 10 13 PM" src="https://user-images.githubusercontent.com/84816495/138624343-2e5f2aa4-08c2-4e95-b8a3-7d6fa410c513.png">


As seen from above, the balanced accuracy score is 54.4% for this model.
For high_risk, the precision is only 1% while the sensitivity (recall) is 69%. The F1 score is therefore 0.02. For low_risk, the precision is 100% while the sensitivity (recall) is 40%. The F1 score is therefore 0.57. The sensitivity is low for low_risk in this model because of the high number of false positives.


### ___Combination Sampling using SMOTEENN___


### ___Balanced Random Forest Classifier___


### ___Easy Ensemble AdaBoost Classifier___

## Summary

Overall, in assessing credit risk, we want to ensure that we detect everyone that is high-risk, even if there will be false positives, than incorrectly characterizing a loan application to be low-risk. This means that high sensitivity for the high-risk assessment is more important than precision in the detection process.
