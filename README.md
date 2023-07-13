## Bootstrapping for Regression Tasks
Author: Andrew Kwon

## Description
This project trains a linear regression model to make predictions from bootstrapped samples. Python code, analysis, and solution contained in Jupyter notebook.

## Introduction
In this project, we are working for a mining company to find the best place for a new oil well. Given a set of data, we will build a linear regression model that will predict the volume of oil reserves for new wells. Our goal is to select the region with the highest profit margin based on the predicted volumes. We will evaluate and justify our selection by calculating the average profit, 95% condience interval and risk of losses (profit loss probability expressed as a percentage).

The following key values used in calculating profits are stored in separate variables to facilitate future scalability and/or modularity:
- *revenue_per_unit*: 4,500 USD per unit of product
- *min_survey_size*: 500 points surveyed per region
- *wells_per_survey*: For each survey, top 200 points selected for profit calculation
- *budget_per_survey*: 100 million USD development budget for 200 wells

## Dataset
Three csv files for each region:

**geo_data_0.csv, geo_data_1.csv, geo_data_2.csv**  
- *id*: unique oil well identifier
- *f0, f1, f2*: three features of points (their specific meaning is unimportant, but the features themselves are significant)
- *product*: volume of reserves in the oil well (thousand barrels)

## Required Libraries
- pandas
- numpy
- sklearn.linear_model
- sklearn.model_selection
- sklearn.metrics
- scipy.stats
