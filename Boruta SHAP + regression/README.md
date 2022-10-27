# Predict industrial parameters with ML model.

In order to optimize production costs, the metallurgical combine LLC "So Temper steel" decided to reduce electricity consumption at the steel processing stage. You have to build a model that predicts the temperature of steel.

## Task

Build a model to predict the output temperature of steel.

## Data
The data consists of files received from different sources:

- `data_arc.csv' — data about electrodes;
- `data_bulk.csv' — data on the supply of bulk materials (volume);
- `data_bulk_time.csv` *—* data on the supply of bulk materials (time);
- `data_gas.csv' — data on gas purging of the alloy;
- `data_temp.csv` — temperature measurement results;
- `data_wire.csv` — data on wire materials (volume);
- `data_wire_time.csv' — data on wire materials (time).



## Brief
- Research analysis of the data:
    - Prepare data, analyze the order of events in the production process, prepare additional fields
- Select the features on which the model will be trained:
    - Generate a number of features
    - Check the features for multicollinearity, exclude unnecessary ones
- Build a model that predicts the temperature of steel:
    -Prepare the procedure for selecting the best model according to the MAE metric and the best hyperparameters for it on several models
     - Perform scaling of features
     - Choose the best model and optimal parameters of OPTUNA c CrossValidation
     - Perform an analysis on train with CrossValidation of the significance of the features and leave only the significant ones
    - Check the effectiveness of the best model on a test sample
    - Build a SHAP diagram of the significance of features on a test sample

## Libraries used

- pandas
- seaborn
- numpy
- matplotlib
- sklearn
- lightgbm
- optuna
- shap
- borutashap
