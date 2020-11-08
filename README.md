# COMPAS-Recidivism-Racial-Bias

COMPAS (Correctional Offender Management Profiling for Alternative Sanctions) is a popular commercial algorithm used by judges and parole officers for scoring criminal defendant’s likelihood of reoffending (recidivism). It has been shown that the algorithm is biased in favor of white defendants, and against black inmates, based on a 2 year follow up study (i.e who actually committed crimes or violent crimes after 2 years). The pattern of mistakes, as measured by precision/sensitivity is notable.

# Results

# Exploratory Data Analysis

## Age

![Age](https://github.com/cv261/COMPAS-Recidivism-Racial-Bias/blob/main/Images/Age.png)

## Custody Status

![Custody Status](https://github.com/cv261/COMPAS-Recidivism-Racial-Bias/blob/main/Images/Custody_Status.png)

## Legal Status

![Legal Status](https://github.com/cv261/COMPAS-Recidivism-Racial-Bias/blob/main/Images/Legal_Status.png)

## Marital Status

![Marital Status](https://github.com/cv261/COMPAS-Recidivism-Racial-Bias/blob/main/Images/Marital_Status.png)

## Race

![Race](https://github.com/cv261/COMPAS-Recidivism-Racial-Bias/blob/main/Images/Race.png)

## Sex

![Sex](https://github.com/cv261/COMPAS-Recidivism-Racial-Bias/blob/main/Images/Sex.png)

# Machine Learning Models

Nearest Neighbors 0.6123110151187905
Linear SVM 0.652267818574514
RBF SVM 0.6641468682505399
Decision Tree 0.6754859611231101
Random Forest 0.6673866090712743
Neural Net 0.6749460043196545
AdaBoost 0.66792656587473
Naive Bayes 0.6241900647948164
QDA 0.6452483801295896
LogisticRegression 0.6652267818574514

Decision Tree model performs the best 

DecisionTreeClassifier(criterion='entropy', max_features=6, min_samples_leaf=8)

     precision    recall  f1-score   support

           0       0.68      0.75      0.71      1020
           1       0.65      0.57      0.61       832

    accuracy                           0.67      1852
   macro avg       0.67      0.66      0.66      1852
weighted avg       0.67      0.67      0.67      1852


