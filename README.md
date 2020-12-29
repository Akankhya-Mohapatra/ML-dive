# Machine Learning-Project
Input file can be downloaded from below link:
https://www.kaggle.com/mlg-ulb/creditcardfraud

The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

Traditionally, we could begin with any number of ways to explore and then decide on a particular technique to classify the fraud transactions and use a performance metric to justify the results. I have implemented K-Means SMOTE with ANN to classify the fraudulent transactions. Then, using confusion matrix, I estimate the f1-score and AUC using the ROC curve.

I initiate with scaling the features followed by K-Means SMOTE to oversample the class samples. Then, I use Neural Networks to produce output with 'relu' activation function in hidden layers and 'sigmoid' in output layers. In this particular use case, I decide on f1-score performance metric because of our primary focus on FP and FN rates. Also, AUC score is a common performance metric used in classification problems.

Note- I applied the oversampling method only to the training set to avoid contaminating the test dataset. The test data set has been utilized to evaluate the F1 score on K-Means SMOTE applied dataset and without.

You will find attached the code implemented to achieve the end goal of classification along with a poster presentation presented to Prof. Laurent Charlin at HEC Montreal and a summarized report on findings and conclusions submitted.
