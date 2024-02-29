# Credit Card Fraud Detection
The aim of this project is to predict whether a given transaction is fraudelent or not based on the information given regarding the transaction. Information such as the transaction amount, card type, product category, etc is given.

In this notebook, I will be visualizing and exploring these features in-depth using seaborn. I will attempt to make inferences and conlusions based on these graphs and plots.

Then, I will demonstrate how to build models to solve this problem. Specifically, I will be using LightGBM and Neural Network models. I will train these models on the training data, and then finally, I will show how to make predictions on the test data using these trained models.

# Data Description
The data is broken into two files identity and transaction, which are joined by TransactionID. Not all transactions have corresponding identity information.

### Categorical Features - Transaction
- ProductCD
- card1 - card6
- addr1, addr2
- P_emaildomain
- R_emaildomain
- M1 - M9

### Categorical Features - Identity
- DeviceType
- DeviceInfo
- id_12 - id_38

The `TransactionDT` feature is a timedelta from a given reference datetime (not an actual timestamp).

You can read more about the data from this post by the competition host.

Files
train_{transaction, identity}.csv - the training set
test_{transaction, identity}.csv - the test set (you must predict the isFraud value for these observations)
sample_submission.csv - a sample submission file in the correct format


