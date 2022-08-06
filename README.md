# Credit_Risk_Analysis

## Overview:

Credit risk is the possibility of loss resulting from non-repayment. Good loans usually outnumber bad loans. We will need employ different techniques to train and evaluate models with unbalances scales. Using the credit card dataset from LendingClub, a peer lending servicers company, we’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. 

Then, we’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results:

![oversampling](https://github.com/AnureetKaurVirdi/Credit_Risk_Analysis/blob/main/Images/oversampling.png)

As displayed on Fig 1, below some remarks:

- The accuracy score is around **65%**
- The precision for High_Risk is = **0.01**
- The precision for Low_Risk is = **1**
- The recall for High_Risk is too low = **0.61**
- The recall for Low_Risk is too high = **0.69**

#### **SMOTE Oversampling**

> *Fig 2: SMOTE oversampling*

![smote](https://github.com/AnureetKaurVirdi/Credit_Risk_Analysis/blob/main/Images/smote_over.png)

Analysing Fig 2, below some remarks:

- The accuracy score is around **64%**
- The precision for High_Risk is too low = **0.01**
- The precision for Low_Risk is too high = **1**
- The recall for High_Risk is = **0.62**
- The recall for Low_Risk is = **0.65**

#### **Cluster Centroids Undersampling**

> *Fig 3: Undersampling*

![undersampling](https://github.com/AnureetKaurVirdi/Credit_Risk_Analysis/blob/main/Images/Undersampling.png)

For Fig 3, we have the following remarks:

- The accuracy score is around **53%**
- The precision for High_Risk is too low = **0.01**
- The precision for Low_Risk is too high = **1**
- The recall for High_Risk is = **0.61**
- The recall for Low_Risk is = **0.45**

#### **SMOTEENN**

> *Fig 4: SMOTEENN*

![smoteenn](https://github.com/AnureetKaurVirdi/Credit_Risk_Analysis/blob/main/Images/smoteenn.png)

From Fig 4, we extract the following remarks:

- The accuracy score is around **62%**
- The precision for High_Risk is too low = **0.01**
- The precision for Low_Risk is too high = **1**
- The recall for High_Risk is = **0.70**
- The recall for Low_Risk is = **0.54**


### **Ensemble Classifiers**

✅ **[Deliverable 3]**

#### **Balanced Random Forest**

> *Fig 5: Balanced Random Forest*

![brf](https://github.com/AnureetKaurVirdi/Credit_Risk_Analysis/blob/main/Images/brf.png)

From Fig 5, we can remark the following:

- The accuracy score is around **78%**
- The precision for High_Risk is = **0.04**
- The precision for Low_Risk is = **1**
- The recall for High_Risk is = **0.67**
- The recall for Low_Risk is = **0.91**

#### **Easy Ensemble Classifier**

> *Fig 6: Easy Ensemble*

![eec](https://github.com/AnureetKaurVirdi/Credit_Risk_Analysis/blob/main/Images/eec.png)

After Fig 6, we have the following remarks:

- The accuracy score is around **93%**
- The precision for High_Risk is = **0.07**
- The precision for Low_Risk is = **1**
- The recall for High_Risk is = **0.91**
- The recall for Low_Risk is = **0.94**

## Summary:

It is important to mention that the original dataset had mayority of the applicatios classified as "Low Risk" and minority as "High Risk" category; with this classification the results would be highly affected and there is a risk that the `Machine Learning` algorithms are creting clusters from too small datasets of "High Risk" applications.
