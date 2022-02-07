# Credit_Risk_Analysis

## Overview
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Resources
* Dataset:

 -LoanStats_2019Q1.csv 

* Software used:

-Python

-Jupyter Notebook

-NumPy, scikit-learn, and imbalanced-learn libraries

-Logistic Regression and Random Forest models

-Ensemble and resampling techinques

## Results
* Naive Random Oversampling:
![image](https://user-images.githubusercontent.com/31675832/152878953-71f7761f-d2ef-4d86-a82f-513f893dccbf.png)

* SMOTE model

![image](https://user-images.githubusercontent.com/31675832/152879280-5f804835-72b2-4183-868b-0b056a826330.png)

* ClusterCentroids model

![image](https://user-images.githubusercontent.com/31675832/152879496-4d175fc4-860f-4cf2-aa74-778e061d9184.png)

* SMOTEENN model

![image](https://user-images.githubusercontent.com/31675832/152879654-e48d8a39-6249-45ee-98a5-b88c5519694e.png)

* BalancedRandomForestClassifier model

![image](https://user-images.githubusercontent.com/31675832/152879881-c48a5df4-5eae-48d8-8b24-306d87ab2dae.png)

* EasyEnsembleClassifier model

![image](https://user-images.githubusercontent.com/31675832/152879979-4664356e-2de6-4198-a40d-8cfa63596a53.png)

## Summary
All the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high.
After factoring in these three main statistics, the model that I would recommend to use for predicting high risk loans is the Easy Ensemble Classifying model.The EasyEnsembleClassifier model shows a recall of 92% so it detects almost all high risk credit. On another hand, with a low precision, a lot of low risk credits are still falsely detected as high risk which would penalize the bank's credit strategy and infer on its revenue by missing those business opportunities.
