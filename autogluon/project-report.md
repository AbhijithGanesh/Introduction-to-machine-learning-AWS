# Report: Predict Bike Sharing Demand with AutoGluon Solution

Submitted by: Abhijith Ganesh

## Initial Training

### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?

I realized that some columns were redundant and had to be dropped for the predictor to work. It was also obvious that for [WeightedEnsemble_L2](https://www.annualreviews.org/doi/10.1146/annurev-biophys-070816-033834) I didn't have a lot of option to modify using hyperparameters.

### What was the top ranked model that performed?

WeightedEnsemble_L2

## Exploratory data analysis and feature creation

### What did the exploratory analysis find and how did you add additional features?

The correlation values of casual, registered was way too high and It added up to count.

### How much better did your model preform after adding additional features and why do you think that is?

It performed better after dropping.

## Hyper parameter tuning

### How much better did your model preform after trying different hyper parameters?

There are no possible HyperParameteres for LightGBM as it defined [here](https://github.com/autogluon/autogluon/blob/master/tabular/src/autogluon/tabular/configs/hyperparameter_configs.py) hence I just had to amend the batch size

### If you were given more time with this dataset, where do you think you would spend more time?

I'd focus on trying fitting various regression models.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score

DOES NOT APPLY.

### Create a line plot showing the top model score for the three (or more) training runs during the project

TODO: Replace the image below with your own.

![model_train_score.png](img/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project

TODO: Replace the image below with your own.

![model_test_score.png](img/model_test_score.png)

## Summary

It would've been more useful and helpful is LightGBM had hyper parameters in the AutoGluon package as it didn't allow me to do much otherwise.
