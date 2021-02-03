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

Following the data exploration section, a linear regression model is
expected to provide weak results as the data involved showed very low
correlations. Nonetheless using it as a part of the model set would
provide a foundation for improvement.

The fitted model is of the form:

$$ OrdersPerHour_t = \beta_0 + \beta_1 EST_ACT_Diff + \beta_2
ITEM_COUNT + \beta_3 ESTIMATED_DELIVERY_MINUTES + \beta_4
ACTUAL_DELIVERY_MINUTES + \beta_5 CLOUD_COVERAGE + \beta_6 TEMPERATURE
+ \beta_7 WIND_SPEED + \beta_8 PRECIPITATION + \beta_9 USER_VENUE_DIST
+ \beta_10 DayOfWeek $$

{% raw %}
  $$a^2 + b^2 = c^2$$ --> note that all equations between these tags will not need escaping! 
 {% endraw %}


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

