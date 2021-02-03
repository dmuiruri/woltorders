[Introduction](./index.md) | [Exploratory Analysis](./docs/assets/pages/data_exploration.md) | [Forecasting Orders](./docs/assets/pages/order_forecasting.md) |[Classifying Orders](./docs/assets/pages/order_classification.md)

# Introduction

In this project data from a food delivery app is analysed with the
purpose of generating insights and creating a prediction model. The
data contains 18706 observations and 12 features as listed below.

## Data Overview

The original data contains metrics related to order delivery and
select weather metrics. The list below shows variables/features
contained in the raw data.

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

### Feature Engineering

In general, we use the available features to generate extra features
that would be useful in providing insights either extra insights or
could be used to enhance modelling algorithms.

Features such as  USER_LAT, USER_LONG, VENUE_LAT, VENUE_LONG are used to
compute the distance between the user and venue, 

- USER_VENUE_DIST (Distance between user and venue)
- DayOfWeek (Day of the week)
- user_coordinates, venue_coordinates (estimated user location)
- venue_postal_code, user_postal_code (estimated venue location)
- source_of_order_pcode (postal code associated with location)
- Orders per hour (Orders issued/received in a given hour
- Source of order based on postal code (A classification feature
  (IN/OUT) used to indicate whether an order came from within the
  postal code or an area outside the postal code