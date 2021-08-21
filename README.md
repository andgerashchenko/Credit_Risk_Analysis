# Credit_Risk_Analysis

The purpose of the analysis is to find the most accurate machine learning model by testing them over the same data set. 

First of all we've tested Logistic Regression model with the different oversampling methods. 
- Here is the results of [Naive Random Oversampling method](https://github.com/andgerashchenko/Credit_Risk_Analysis/blob/700daf3d34639c0356e30569bbdbdf66d815724b/Resources/Naive%20Random%20Oversampling.png).
Accuracy score - 0.65, which is not good. Recall is also pretty low (0.66) for both high and low risk values, while precision is prerfect (1.0) for high and just 0.01 for low risk.
- [SMOTE oversampling method](https://github.com/andgerashchenko/Credit_Risk_Analysis/blob/master/Resources/SMOTE%20Oversampling.png) shows similar picture. 
Accuracy score - 0.63, recall - 0.62 and 0.66 for high and low risk accordingly. Precision is the same as Naive Random.
- Then we tried to decrease larger part of the data rather then increase smaller. [Undersampling method](https://github.com/andgerashchenko/Credit_Risk_Analysis/blob/700daf3d34639c0356e30569bbdbdf66d815724b/Resources/Undaersampling.png) gives even worse output.
Accuracy - 0.53, recall 0.61 and 0.45 for hihg and low accordingly, and the same precision values (1.0 and 0.01).
- [Combination Sampling](https://github.com/andgerashchenko/Credit_Risk_Analysis/blob/700daf3d34639c0356e30569bbdbdf66d815724b/Resources/Combination%20Sampling.png) makes a little improvement in recall for high risk (0.70), but it's still moderate. 
As well as other values: Accuracy - 0.64, low risk recall - 0.57 and precision - 0.01 and 1.0 for high and low risk.
- Finally we ran deep learning models. [Balanced Random Forest Classifier](https://github.com/andgerashchenko/Credit_Risk_Analysis/blob/700daf3d34639c0356e30569bbdbdf66d815724b/Resources/Balance%20Random%20Forest%20Classifier.png) was first.
Almost all the values shows perceptible increase. Accuracy score - 0.78, recall - 0.68 and 0.89 for high and low risk accordingly. 
And at last we can see slightly growth of precision for high risk, which is 0.03 now.
- The last model we used is [Easy Ensemble AdaBoost Classifier](https://github.com/andgerashchenko/Credit_Risk_Analysis/blob/master/Resources/Easy%20Ensemple%20Classifier.png), which combined 100 estimators. And this time our model proved to be reliable. 
Accuracy score - 0.92, Precision - 0.08 and 1.0, Recall - 0.91 and 0.94 for high and low risk accordingly.
