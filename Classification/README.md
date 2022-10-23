# Bootstrap in oil mining company

Customers began to leave BetaBank. Every month. A little, but noticeable. Bank marketers have calculated that it is cheaper to retain current customers than to attract new ones.

## Task
Predict whether the client will leave the bank in the near future or not. You have historical data on the behavior of customers and the termination of contracts with the bank.
Build a model with an extremely large value of F1-measures. Bring the metric to 0.59+.

## Data
Data source: [kaggle.com](https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling)

Features
- RowNumber — index of the row in the data
- CustomerID — unique customer ID
- Surname — surname
- CreditScore — credit rating
- Geography — country of residence
- Gender — gender
- Age — age
- Tenure — how old is a person a bank customer
- Balance — account balance
- NumOfProducts — number of bank products, used by the client
- HasCrCard —has credit card
- IsActiveMember — client activity
- EstimatedSalary —estimated salary

Target
- Exited — the fact of the client's leaving

## Brief
- We loaded data, evaluated it.
- Try 3 models without elimination of imbalance
- Try the same 3 models with 4 ways for elimination of imbalance (optimal treshold, downsampling, upsampling, balancing)
- make conclusions


## Libraries used

- pandas
- numpy
- seaborn
- matplotlib
- sklearn
- imblearn