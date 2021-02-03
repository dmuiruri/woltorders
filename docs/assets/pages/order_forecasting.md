[Introduction](./../../index.md) | [Exploratory Analysis](./../pages/data_exploration.md) | [Forecasting Orders](./../pages/order_forecasting.md) |[Classifying Orders](./../pages/order_classification.md)

# Forecasting

Being able to forecast the amount of orders has the potential to
improve business efficiency, so the objective of this section was to
forecast the amount of incoming orders. 4 different models were
developed and tuned and their results compared

- A linear regression model
- A linear regression with dummy variables
- A regression tree model
- An ARIMA model

The main variable being predict(endog) is number of orders. This
variable is created by aggregating the amount of orders obtained per
day or per hour depending with the use case.

## Linear Regression model

Following the data exploration section, this model is expected to
provide weak results as the data involved showed very low
correlations. Nonetheless using it as a part of the model set would
provide a foundation for improvement.



[back to top](./../pages/order_forecasting.md)

## A Linear regression model with dummy variables

Since weekdays were shown to have different order patterns, this model
explores if this patterns would result in a reasonable prediction
model.

[back to top](./../pages/order_forecasting.md)


## A Regression Decision Tree Model
Regression trees are considered a good non-parametetric approach to this problem

[back to top](./../pages/order_forecasting.md)

## A ARIMA Model

Given that the data indicated highly cyclic characteristics, it is
imperative that we test a dedicatedtimeseries model on the data.

[back to top](./../pages/order_forecasting.md)

