# Credit-card-fraud
DESCRIPTION

Problem Statement:Finance Industry is the biggest consumer of Data Scientists. It faces constant attack by fraudsters, who try to trick the system. Correctly identifying fraudulent transactions is often compared with finding needle in a haystack because of the low event rate. It is important that credit card companies are able to recognize fraudulent credit card transactions so that the customers are not charged for items that they did not purchase. You are required to try various techniques such as supervised models with oversampling, unsupervised anomaly detection, and heuristics to get good accuracy at fraud detection. 

The datasets contain transactions made by credit cards in September 2013 by European cardholders. This dataset represents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

Downlod the data sets from : https://www.dropbox.com/s/6z5jxcqaqipxiun/Project%202-Finance-Datasets.zip?dl=0

Project Task

Exploratory Data Analysis (EDA):
Perform an EDA on the Dataset. 
a) Check all the latent features and parameters with their mean and standard deviation. Value are close to 0 centered (mean) with unit standard deviation 
b) Find if there is any connection between Time, Amount, and the transaction being fraudulent.

Check the class count for each class. It’s a class Imbalance problem.

Use techniques like undersampling or oversampling before running Naïve Bayes, Logistic Regression or SVM. 
  a. Oversampling or undersampling can be used to tackle the class imbalance problem 
  b. Oversampling increases the prior probability of imbalanced class and in case of other classifiers, error gets multiplied as the low-proportionate class is mimicked multiple times. 
 
  Following are the matrices for evaluating the model performance:
  Precision, Recall, F1-Score, AUC-ROC curve. Use F1-Score as the evaluation criteria for this project.

Note: Major terms used with AUC and ROC Curve
Let us consider :

TP - True Positive
FP - False Negative
TN - True Negative
FP - False Negative
Now, the classification report will calculate the below values for evaluating each model :

1. Precision :
Precision=TPTP+FP=TPTotalPredictedPossitive

2. Sensitivity or Recall or TPR (True Positive Rate) :
TPR/Recall/Sensitivity=TPTP+FN=TPTotalTotalActualPositive

3. Specificity :
Specificity=TNTN+FP

4. FPR (False Positive Rate) or TNR (True Negative Rate) :
TPRorFPR=1−Specificity=1−(TNTN+FP)=FPTN+FP

5. F1-Score :
F1=1∗(Precision∗RecallPrecision+Recall)


Modeling Techniques:
Try out models like Naive Bayes, Logistic Regression or SVM. Find out which one performs the best Use different Tree-based classifiers like Random Forest and XGBoost.

   a.    Remember Tree-based classifiers work on two ideologies: Bagging or Boosting
   b.    Tree-based classifiers have fine-tuning parameters which takes care of the imbalanced class. Random-Forest and XGBboost.

Compare the results of 1 with 2 and check if there is any incremental gain.

##### Comparing the results of undersmpled data from all 04 modelling techniques namely Logistic Regression, Naive Bayes, Random Forest & XGBoost in a sequencial manner, providing a rank.
###### 1. RandomForestClassifier for bagging (acc_score=0.99, f1_score=0.31, precision=0.19, recall=0.84)
###### 2. XGBoost Classifier (acc_score=0.97, f1_score=0.10, precision=0.05, recall=0.89)
###### 3. Logistic Regression (acc_score=0.97, f1_score=0.09, precision=0.04,recall=0.89)
###### 4. Naive Bayes Classifier(acc_score=0.98,f1_score=0.10, precision=0.11, recall=0.71)


Applying ANN:
###### Use ANN (Artificial Neural Network) to identify fradulent and non-fradulent.

a)    Fine-tune number of layers
b)    Number of Neurons in each layers
c)    Experiment in batch-size
d)    Experiment with number of epochs. Check the observations in loss and accuracy
e)    Play with different Learning Rate variants of Gradient Descent like Adam, SGD, RMS-prop
f)    Find out which activation performs best for this use case and why?
g)    Check Confusion Matrix, Precision, Recall and F1-Score
Try out Dropout for ANN. How is it performed? Compare model performance with the traditional ML based prediction models from above.

Find the best setting of neural net that can be best classified as fraudulent and non-fraudulent transactions. Use techniques like Grid Search, Cross-Validation and Random search.
###### Anomaly Detection:
Implement anomaly detection algorithms. 
a) Assume that the data is coming from a single or a combination of multivariate Gaussian 
b) Formalize a scoring criterion, which gives a scoring probability for the given data point whether it belongs to the multivariate Gaussian or Normal Distribution fitted in a)

###### Inference and Observations:
Visualize the scores for Fraudulent and Non-Fraudulent transactions.
Find out the threshold value for marking or reporting a transaction as fraudulent in your anomaly detection system.
Can this score be used as an engineered feature in the models developed previously? Are there any incremental gains in F1-Score? Why or Why not?
Be as creative as possible in finding other interesting insights.
Visualizing the fraudalent and non-fradaulant transcation after anomaly or outlier removal from undersampled data.

#### Observations:
