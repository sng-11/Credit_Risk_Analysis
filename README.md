# Credit Risk Analysis

## Overview of the Project
Assessing credit risk is an important endeavour conducted by organizations before issuing loans to their applicants. The applicant must be evaluated over many different criteria to ensure that they have the ability to pay back the loan in the future. Because of the huge amount of data involved in this process, it is useful to use machine learning models to learn from pre-existing data and develop algorithms that can be applied to future loan applications. As such, this project uses a variety of models from the imbalanced-learn and scikit-learn libraries to conduct resampling and assess credit risk.

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
For high_risk, the precision is only 1% while the sensitivity (recall) is 63%. The F1 score is therefore 0.02. For low_risk, the precision is 100% while the sensitivity (recall) is 69%. The F1 score is therefore 0.82.


### ___Undersampling with Cluster Centroids___

<img width="450" alt="Screen Shot 2021-10-24 at 9 58 04 PM" src="https://user-images.githubusercontent.com/84816495/138623462-42ef2523-9fb9-4f1e-bd26-849814d2a3f1.png">
<img width="709" alt="Screen Shot 2021-10-24 at 10 10 13 PM" src="https://user-images.githubusercontent.com/84816495/138624343-2e5f2aa4-08c2-4e95-b8a3-7d6fa410c513.png">


As seen from above, the balanced accuracy score is 54.4% for this model.
For high_risk, the precision is only 1% while the sensitivity (recall) is 69%. The F1 score is therefore 0.02. For low_risk, the precision is 100% while the sensitivity (recall) is 40%. The F1 score is therefore 0.57. The sensitivity is low for low_risk in this model because of the high number of false positives.


### ___Combination Sampling using SMOTEENN___

<img width="451" alt="Screen Shot 2021-10-24 at 10 21 00 PM" src="https://user-images.githubusercontent.com/84816495/138625194-57302cb0-140b-47d3-b821-21df1a88e9b7.png">
<img width="716" alt="Screen Shot 2021-10-24 at 10 21 18 PM" src="https://user-images.githubusercontent.com/84816495/138625216-ca8ae14c-b99d-486d-b095-32e4fbaedebc.png">

As seen from above, the balanced accuracy score is 64.5% for this model.
For high_risk, the precision is only 1% while the sensitivity (recall) is 72%. The F1 score is therefore 0.02. For low_risk, the precision is 100% while the sensitivity (recall) is 57%. The F1 score is therefore 0.73.


### ___Balanced Random Forest Classifier___

<img width="366" alt="Screen Shot 2021-10-24 at 10 13 55 PM" src="https://user-images.githubusercontent.com/84816495/138624615-54bb1d58-894a-4c05-a8c2-93ffdfb225a4.png">
<img width="707" alt="Screen Shot 2021-10-24 at 10 14 09 PM" src="https://user-images.githubusercontent.com/84816495/138624636-0c2f4024-173e-4f79-b379-64d8e649ea49.png">

As seen from above, the balanced accuracy score is 78.9% for this model.
For high_risk, the precision is only 3% while the sensitivity (recall) is 70%. The F1 score is therefore 0.06. For low_risk, the precision is 100% while the sensitivity (recall) is 87%. The F1 score is therefore 0.93. 
According to the this model, the important features include total_rec_prncp and total_pymnt. 


### ___Easy Ensemble AdaBoost Classifier___

<img width="371" alt="Screen Shot 2021-10-24 at 10 17 27 PM" src="https://user-images.githubusercontent.com/84816495/138624898-e1db0275-67be-4db5-877d-957c5432ec23.png">
<img width="713" alt="Screen Shot 2021-10-24 at 10 17 43 PM" src="https://user-images.githubusercontent.com/84816495/138624919-f854399a-3367-480d-b6b3-20c69f9866bb.png">

As seen from above, the balanced accuracy score is high for this model, at 93.2%.
For high_risk, the precision is 9% while the sensitivity (recall) is 92%. The F1 score is therefore 0.16. For low_risk, the precision is 100% while the sensitivity (recall) is 57%. The F1 score is therefore 0.73. 


## Summary

Overall, in assessing credit risk, we want to ensure that we detect everyone that is high-risk, even if there will be false positives, than incorrectly characterizing a loan application to be low-risk. This means that high sensitivity for the high-risk assessment is more important than precision in the detection process.
