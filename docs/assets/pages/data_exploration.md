[Introduction](./../../index.md) | [Exploratory Analysis](./../pages/data_exploration.md) | [Forecasting Orders](./../pages/order_forecasting.md) |[Classifying Orders](./../pages/order_classification.md)

# Data Overview

This section investigates the relationships between features and the
individual characteristics of the variables of interest.

## Correlations

The matrix of correlations between variables indicates that most
variables have low correlations, meaning no structural causality can
be generated variables in their current form.

![Correlations](../images/correlations_wolt.png)

The image below shows the scatter plots of individual variables
against each other. As the scatter plots show, most variables do not
have a strong linear relationship among each other. Additionally, the
KDE plots show characterisitcs of the variables, only the EST_ACT_Diff
shows signs of a normal distributions while others have non-normal
distributions.

![scatterplot](../images/scatter_kde_plots.png)

## Distributions plots of Key Variables

The distribution of USER_VENUE_DIST shows that the average distance
between users and venue is about 1Km (1.02), the plot also shows a
tendancy to have distances that are further than 2Kms. ITEM_COUNT
distribution shows that orders with 1 item are dominant (average 2.6
items), interestingly, some orders may though rare may have more than
4 items. The EST_ACT_Diff variable represents the difference in
minutes between estimated time for a delivery and the actual time it
takes for the delivery to be completed. The distribution is
interestingly almost centered around zero (-1.2) but also shows signs
of under/over estimation of the time required to deliver the meals.


![distplot](../images/distribution_uservenue_itemcount_dist.png)
[back](./../pages/data_exploration.md)
