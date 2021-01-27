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

Features, USER_LAT, USER_LONG, VENUE_LAT, VENUE_LONG are used to
compute the distance between the user and venue.