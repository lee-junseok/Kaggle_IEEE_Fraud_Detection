# Fraud_Transaction_Detection
This is a short machine learning project to detect fraud transaction.

Transaction Data from the Kaggle Competition "IEEE Fraud Detection"

Competition overview:

'''

In this competition you are predicting the probability that an online transaction is fraudulent, as denoted by the binary target isFraud.

The data is broken into two files identity and transaction, which are joined by TransactionID. Not all transactions have corresponding identity information.

Categorical Features - Transaction
ProductCD
card1 - card6
addr1, addr2
P_emaildomain
R_emaildomain
M1 - M9
Categorical Features - Identity
DeviceType
DeviceInfo
id_12 - id_38
The TransactionDT feature is a timedelta from a given reference datetime (not an actual timestamp).

You can read more about the data from this post by the competition host.

Files
train_{transaction, identity}.csv - the training set
test_{transaction, identity}.csv - the test set (you must predict the isFraud value for these observations)
sample_submission.csv - a sample submission file in the correct format

'''

Files:


- requirements.txt contains packages used this work.

- Kaggle_IEEE_Fraud_Detection_EDA contains data exploring and feature engineering ideas with plots.

- Kaggle_IEEE_Fraud_Detection_Model contains data preprocessing, feature engineering, modeling and prediction.

The baseline model with simple data preprocessing and modeling with RandomForest Classifier gives an AUC score 0.8783. My work with Lightgbm improved it by 11.1% and got an AUC score 0.97552.
