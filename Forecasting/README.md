# Forecasting taxi orders

The company "An awesome taxi" collected historical data on taxi orders at airports. To attract more drivers during peak load, you need to predict the number of taxi orders for the next hour.


## Task
Build a model for such a prediction. 
Train different models with different hyperparameters. Make a test sample of 10% of the original data.
Check the data on the test sample and draw conclusions.

## Data
The data is in the file 'taxi.csv'. The number of orders is in the num_orders column

## Brief
- We loaded data, evaluate and prepare it for further analysis. 
- We perform stationarity tests (KPSS & ADF), 
- Evaluate periods by FFT and ACF & PACF,
- Define type of seasonality and type of trend
- Generate features for regression models
- Test models: Linear Regression, LGBM, SARIMA, HoltWinters, SLT Forecast, Facebook Prophet
- Select best model on validation dataset and test it on test dataset


## Libraries used

- pandas
- scipy
- numpy
- seaborn
- matplotlib
- statsmodels
- time
- datetime
- sklearn
- scipy
- lightgbm
- tqdm
- prophet
