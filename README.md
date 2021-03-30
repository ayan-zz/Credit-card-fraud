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
