# Credit_Risk_Analysis

## Purpose of Analysis
This project folder contains two separate Jupyter Notebook files: credit_risk_resampling and credit_risk_ensemble. Credit_risk_resampling preprocesses information about a client's loan application, splits the data into training and testing data, and then performs several resampling techniques designed to address an imbalanced dataset, and runs a standard logistic regression machine learning model to analyze the performance of the different resampling techniques Note that the loan application dataset is imbalanced due to large number of "low-risk" loans and the low number of "high-risk" loans. The logistic regression attempts to predict whether a particular loan application is either low-risk or high-risk based on the myriad of training variables such as loan amount, annual income, the interest rate on the loan. 

First, I used both a naive random oversampling algorithm and then a synthetic minority oversampling technique (SMOTE) algorithm, running both through the logistic regression model. Then I tried using undersampling with a cluster centroid undersampling algorithm and used a combination of over and under sampling with a SMOTEEN (SMOTE + Edited Nearest Neighbors (ENN)) sampling algorithm, running both through the logistic regression model as well. For each sampling technique, I calculated a balanced accuracy score, a confusion matrix, and a imbalanced classification report to analyze the performance of each resampling technique. 

In the Credit_risk_ensemble file, I do the same preprocessing work on the data, split the data into training and test sets, and then run both a Balanced Random Forest Classifier model and a Easy Ensemble AdaBoost Classifier model to see which one performed better. Below, I will discuss the results of the different sampling techniques and the two machine learning models mentioned just above as well as provide a summary of the results and a recommendation on which model to use for predicting credit risk from loan application information.

## Results
### Naive Random Oversampling
* Balanced Accuracy Score

![Random Oversampling Accuracy](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/Random%20Oversampling%20Accuracy.png)

* Confusion Matrix

![Random Oversampling Confusion Matrix](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/Random%20Oversampling%20Confusion%20Matrix.png)

* Imbalanced Classification Report

![Random Oversampling Classification Report](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/Random%20Oversampling%20Classification%20Report.png)

### SMOTE Oversampling
  * Balanced Accuracy Score

![SMOTE Oversampling Accuracy](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/SMOTE%20Accuracy.png)

  * Confusion Matrix

![SMOTE Oversampling Confusion Matrix](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/SMOTE%20Confusion%20Matrix.png)

  * Imbalanced Classification Report

![SMOTE Oversampling Classification Report](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/SMOTE%20Classification%20Report.png)

### Cluster Centroids Undersampling
* Balanced Accuracy Score

![Undersampling Accuracy](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/Undersampling%20Accuracy.png)

* Confusion Matrix

![Undersampling Confusion Matrix](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/Undersampling%20Confusion%20Matrix.png)

* Imbalanced Classification Report

![Undersampling Classification Report](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/Undersampling%20Classification%20Report.png)

### SMOTEENN
* Balanced Accuracy Score

![SMOTEENN Accuracy](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/SMOTEEN%20Accuracy.png)

* Confusion Matrix

![SMOTEENN Confusion Matrix](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/SMOTEEN%20Confusion%20Matrix.png)

* Imbalanced Classification Report

![SMOTEENN Classification Report](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/SMOTEEN%20Classification%20Report.png)

### Balanced Random Forest Classifier   
* Balanced Accuracy Score

![BRFC Accuracy](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/Balanced%20Random%20Forest%20Accuracy.png)

* Confusion Matrix

![BRFC Confusion Matrix](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/Balanced%20Random%20Forest%20Confusion%20Matrix.png)

* Imbalanced Classification Report

![BRFC Classification Report](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/Balanced%20Random%20Forest%20Classification%20Report.png)

### Easy Ensemble AdaBoost Classifier
* Balanced Accuracy Score

![Easy Ensemble Accuracy](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/Easy%20Ensemble%20Accuracy.png)

* Confusion Matrix

![Easy Ensemble Accuracy](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/Easy%20Ensemble%20Confusion%20Matrix.png)

* Imbalanced Classification Report

![Easy Ensemble Accuracy](https://github.com/SethBoswell/Credit_Risk_Analysis/blob/main/Images/Easy%20Ensemble%20Classification%20Report.png)

## Summary
### Summary of Results

### Recommendation
