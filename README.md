# Credit_Risk_Analysis
# OverView of the analysis :
 
In this module, we used Python to build and evaluate several machine learning models to predict credit risk. Being able to predict credit risk with machine learning algorithms can help banks and financial institutions predict anomalies, reduce risk cases, monitor portfolios, and provide recommendations on what to do in cases of fraud.
Credit risk is very tough to predict. In this project we want to take a look at how all the factors in our **loan_stats csv** helps to predict whether someone is low or high risk status.

# Purpose :
1.Explain how a machine learning algorithm is used in data analytics.
2. Create training and test groups from a given data set.
3. Implement the logistic regression, decision tree, random forest, and support vector machine algorithms.
4. Interpret the results of the logistic regression, decision tree, random forest, and support vector machine algorithms.
5. Compare the advantages and disadvantages of each supervised learning algorithm.
6. Determine which supervised learning algorithm is best used for a given data set or scenario.
7. Use ensemble and resampling techniques to improve model performance.

Results :
In this module describe the balanced accuracy scores and the precision and recall scores of all six machine learning models.
Here are all six accuracy detalis, below :

1. # Naive Random Oversampling
 . Naive Random Oversampling results: Our balanced accuracy test it 64%, the precision for the high_risk has a very low positivity at 1% and the recall is 60%

 ![Naive_Random_Oversampling)](/Resources/Naive_Random_Oversampling.png)

2. # SMOTE Oversampling
  . SMOTE oversampling results: the accuracy score is 66.2%, the precision for the high_risk loans has a low positvity again at 1% and recall is 69% overall  


 ![SMOTEOversampling)](/Resources/SMOTE_Oversampling.png)

3.# Undersampling
  . Undersampling results: balanced accuracy score is 66.2% overall, the precision is at 99% and the recall is 69%

 ![Undersampling)](/Resources/Undersampling.png)

4. # Combination (Over and Under) Sampling
  . Combination(over and undersampling) results: balanced accuracy score is 66% the precision is 99% and the recall is 57% overall

  ![Combination_Sampling)](/Resources/Combination_Sampling.png)

5. # Balanced Random Forest Classifier
  . Balanced Random Forest Classifier results: the accuracy score is 74.2% the precision is 99% and the recall is 85%

  ![Balanced_Random_Forest_Classifier)](/Resources/Balanced_Random_Forest_Classifier.png)

6.# Easy Ensemble AdaBoost Classifier
  . Easy Ensemble AdaBoost Classifier results: the accuracy score is 93% the precision is 99% and the recall is 94%

  ![Easy_Ensemble_AdaBoost)](/Resources/Easy_Ensemble_AdaBoost.png)


# Summary :
In the first four models we undersampled, oversampled and did a combination of both to try and determine which model is best at predicting which loans are the highest risk. The next two models we resampled the data using ensemble classifiers to try and predict which which loans are high or low risk. In our first four models our accuracy score is not as high as the ensemble classifiers and the recall in the oversampling/undersampling/mixed models is low as well. Typically in your models you want a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models. It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.

