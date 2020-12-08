# Data_Mining_Python
Data mining challenge

Predictive modeling
Goal is to build a model that predicts a probability that a given customer will default on a loan
A customer profile consists of a list of bank transactions preceding the loan request. Each transaction is either a debit
(money going out of account, negative values) or credit (money coming into account, positive values).
Customer profile (attributes) (15000 customers total):
Id – id of each customer
dates – dates of each transaction
transaction_amount – numpy array of credits and debits, length varies across different customers
(your predictions will be primarily based on information in this array)
days_before_request – days before loan request for each transaction
loan_amount – amount loaned to customer by bank
loan_date – date of loan
outcome:
isDefault – did the customer pay back (isDefault=0) or not pay back (isDefault=1)?
isDefault is given for the first 10000 customers. Your job is to assign a probability to isDefault for the remaining 5000
customers.
Train your model on the training data (instances 0 - 9999) and make predictions on the test data (instances 10000-
14,999). The test data is the same format as training data, except it does not contain the isDefault column.
The data can be loaded from dataset.pkl in python using:
import pandas as pd
data = pd.read_pickle('path/to/data/dataset.pkl')
