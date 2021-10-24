# Credit Risk Analysis

## Overview of the Project
Assessing credit risk is an important endeavour conducted by orgnaizations before issuing loans to their applicants. The applicant must be evaluated over many different criteria to ensure that they have the ability to pay back the loan in the future. Because of the huge amount of data involved in this process, it is useful to use machine learning models to learn from pre-existing data and develop algorithms that can be applied to future loan applications. As such, this project uses a variety of models from the imbalanced-learn and scikit-learn libraries to conduct resampling and assess credit risk.

## Results

Six machine learning models were used in this analysis, with an evaluation of each below:

___Naive Random Oversampling___

<img width="583" alt="Screen Shot 2021-10-24 at 4 10 08 PM" src="https://user-images.githubusercontent.com/84816495/138611012-f06a982b-8163-414e-be11-c2634b889eb9.png">
<img width="803" alt="Screen Shot 2021-10-24 at 4 10 29 PM" src="https://user-images.githubusercontent.com/84816495/138611029-56531110-e388-4aee-9648-50759f4bfbd0.png">

As seen from above, the balanced accuracy score is 65.5% for this model.
The 

___Oversampling with SMOTE___


___Undersampling with Cluster Centroids___


___Combination Sampling using SMOTEENN___


___Balanced Random Forest Classifier___


___Easy Ensemble AdaBoost Classifier___

## Summary

Overall, in assessing credit risk, we want to ensure that we detect everyone that is high-risk, even if there will be false positives, than incorrectly characterizing a loan application to be low-risk. This means that high sensitivity for the high-risk assessment is more important than precision in the detection process.
