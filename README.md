# Credit_Risk_Analysis

## Overview of the loan prediction risk analysis:
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I will employ different techniques to train and evaluate models with unbalanced classes. I will use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I will oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I will use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. I will then compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Then I will evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results
For each of the six machine learning models I used I will be displaying my accuracy score, precision, and recall scores for each. The six models include the Naive Random Oversampling model, the SMOTE Oversampling model, an Undersampling model, a Combination model, a Balanced Random Forest Classifier model, and an Easy Ensemble AdaBoost Classifier model. The results for each of these models will be shown below.

* NAIVE Random Oversampling
    * Balanced Accuracy Score: ~ 0.6441
  
![NaiveRandomOversampling](Resources/NaiveRandomOversampling.PNG)
  
* SMOTE Oversampling
  * Balanced Accuracy Score: ~ 0.6483
 
![SMOTEOversampling](Resources/SMOTEOversampling.PNG)
  
* Undersampling
  * Balanced Accuracy Score: ~ 0.6483
  
![Undersampling](Resources/Undersampling.PNG)
  
* Combination (Oversampling and Undersampling)
  * Balanced Accuracy Score: ~ 0.5103
  
![Combination](Resources/Combination.PNG)
  
* Balanced Random Forest Classifier
  * Balanced Accuracy Score: ~ 0.7878
  
![BalancedRandomForestClassifier](Resources/BalancedRandomForestClassifier.PNG)
  
* Easy Ensemble AdaBoost Classifier
  * Balanced Accuracy Score: ~ 0.9254
  
![EasyEnsembleAdaBoostClassifier](Resources/EasyEnsembleAdaBoostClassifier.PNG)


## Summary
Given the results of all six tests, we can see a clear cut best option. the Easy Ensemble Ada Boost Classifier outshined the rest of the field with a Balanced Accuracy score of ~ 0.9254 out of a perfect 1.0000. The next best model, the Combination had a Balanced Accuracy score nearly 0.2000 lower. In addition, the F1 score which tells us the percentage of positive predictions that were correct show that
