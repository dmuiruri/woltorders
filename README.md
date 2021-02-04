# woltorders

This project presents an analysis of data (orders data) from Wolt,
which is a food delivery platform. The data is a snapshot taken from
August - September 2020.

## Summary

The original data contains the following features/variables

- ACTUAL_DELIVERY_MINUTES \- ESTIMATED_DELIVERY_MINUTES
- ITEM_COUNT
- USER_LAT
- USER_LONG
- VENUE_LAT
- VENUE_LONG,
- ESTIMATED_DELIVERY_MINUTES
- ACTUAL_DELIVERY_MINUTES,
- CLOUD_COVERAGE
- TEMPERATURE
- WIND_SPEED
- PRECIPITATION

The analysis includes an exploratory analysis, a regression aspect and
a classification aspect. The regression and classification problems
are aimed at creating a predictive model.

### Exploratory Analysis

The exploratory analysis focuses on studying the characteristics of
selected features and some additional features are derived from the
original dataset. Examples of derived features include distance
between an orders USER and VENUE, a USER's/VENUE estimated location by
postal code is derived by using Google map's reverse geocoding API and
orders per hour. Results in this section indicate orders where only 1
item is ordered are highly common but also orders with 4-10 items do
occur also not frequently. Friday's, Saturday's and Sunday's tend to
be most popular days for orders. Orders within a given day often peak
during the afternoon during lunch hours.

### Prediction modelling

The prediction problem is formulated to predict the number of orders
per hour based on the other variables. Various prediction algorithms
are tested (Linear regression, Linear regression with weekday dummy
variables, a boosted tree and an ARIMA model) where the ARIMA model
provides the best results based on RMSE evaluation (5.72 on test set).

### Classification modelling

The classification setup is formulated to predict whether an order is
originating from within/outside a zone. Two algorithms (logistic
regression and support vector machine) are tested for their
accuracy. The logistic regression shows the highest accuracies of 82%

## Site

The results of these analysis are exhaustively presented on this
[site](https://dmuiruri.github.io/woltorders/) where more details and
relevant graphs are presented.

## Notebook and Data

A corresponding notebook and data can be obtained by downloading the
zip file(wolt_project.zip) in the repository.

Updates will be occassionally added especially in order to improve
certain aspects of modelling.

Suggestions and improvement ideas are welcome, I bet there are many
other ways this project could be improved by either using alternative
libraries or even new angles to solve the tasks.

