# Credit Risk Analysis

The purpose of the analysis is to find the most accurate machine learning model by test them over the same data set. 

First of all we've tested Logistic Regression model with the different oversampling methods. 
- Here is the results of **Naive Random Oversampling method**.
Accuracy score - 0.65, which is not good. Recall is also pretty low (0.66) for both high and low risk values, while precision is perfect (1.0) for high and just 0.01 for low risk.
![Naive Random Oversampling](https://user-images.githubusercontent.com/79814533/138602332-bfee1bea-5915-4762-8c83-df6611523fc2.png)

- **SMOTE oversampling method** shows similar picture. 
Accuracy score - 0.63, recall - 0.62 and 0.66 for high and low risk accordingly. Precision is the same as Naive Random.
![SMOTE Oversampling](https://user-images.githubusercontent.com/79814533/138602348-7b3d7abd-d911-4191-bfe7-f7cf8089a8b4.png)

- Then we tried to decrease larger part of the data rather then increase smaller using **Undersampling method**.
Accuracy - 0.53, recall 0.61 and 0.45 for hihg and low accordingly, and the same precision values (1.0 and 0.01).
![Undaersampling](https://user-images.githubusercontent.com/79814533/138602361-9b1c98ed-5572-4c7d-881a-5668213bc6e1.png)

- **Combination Sampling** makes a little improvement in recall for high risk (0.70), but it's still moderate. 
As well as other values: Accuracy - 0.64, low risk recall - 0.57 and precision - 0.01 and 1.0 for high and low risk.
![Combination Sampling](https://user-images.githubusercontent.com/79814533/138602379-35e32174-23c8-48f6-9562-0d1b1996741f.png)

- Finally we ran ensemble learning models. **Balanced Random Forest Classifier** was first.
Almost all the values shows perceptible increase. Accuracy score - 0.78, recall - 0.68 and 0.89 for high and low risk accordingly. 
And at last we can see slight growth of precision for high risk, which is 0.03 now.
![Balance Random Forest Classifier](https://user-images.githubusercontent.com/79814533/138602395-225012d4-1c66-4f23-92ea-478392816670.png)

- The last model we used is **Easy Ensemble AdaBoost Classifier**. And this time our model proved to be reliable. 
Accuracy score - 0.92, Precision - 0.08 and 1.0, Recall - 0.91 and 0.94 for high and low risk accordingly.
![Easy Ensemple Classifier](https://user-images.githubusercontent.com/79814533/138602414-d20682d1-3836-4726-82ee-913665e77985.png)

Summarizing all the results of used machine learning models we can assume that for this particular type of data ensemble learning models are more suitable, especially Easy Ensemble AdaBoost Classifier. However we can continue trying other models and maybe find better fit, polishing results by fine tune of Easy Ensemble parameters could be more effective. 
