# Prediction rate of gold from gold-bearing ore

The model should predict the recovery rate of gold from gold-bearing ore. Use data with mining and cleaning parameters.


## Task

Build a model to predict the recovery rate of gold from gold-bearing ore. Use data with mining and cleaning parameters.

Predict two values at once:<br>
- the efficiency of enrichment of rough concentrate is rougher.conclusion.recovery;
- the final concentrate enrichment efficiency is final.conclusion.recovery.
The final metric consists of two values:<br><br>
$$\mathit{result_{MAPE}} = 25\%\times \mathit{sMAPE}_{ROUGHER} + 75\%\times \mathit{sMAPE}_{FINAL} $$

## Data
The data of the three regions are in the files: gold_recovery_train_new.csv, gold_recovery_test_new.csv, gold_recovery_full_new.csv

The name of the features should be as follows: [stage].[parameter type].[parameter name]
Example: *rougher.input.feed_ag*

Possible values for the [stage] block:
- rougher — flotation
- primary_cleaner — primary cleaning
- secondary_cleaner — secondary cleaning
- final — final characteristics

Possible values for the [parameter type] block:
- input — raw material parameters
- output — product parameters
- state — parameters characterizing the current state of the stage
- calculation — calculated characteristics

## Brief
- ETL. We loaded data, evaluated it.
- Concentration of metals (Au, Ag, Pb) change at different stages of purification
- Distributions of raw material pellets in the training and test samples
- Total concentration of all substances at different stages
- Select best hyper params for each model
- Select best model on train set
- Check best model on test set
- Final conclusions and Recomendations

## Libraries used

- pandas
- seaborn
- matplotlib
- sklearn
- imblearn
- optuna
- scipy
