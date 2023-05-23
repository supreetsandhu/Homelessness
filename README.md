# Homelessness

## Description
This project will look at the homelessness in the USA. The U.S. Department of Housing and Urban Development (HUD) argues that local market factors are determiants and factors in homelessness. This project is directly motivated by the claim by HUD. This project will look at other models that correlate to local market factors and homelessness, to see if we can produce a model that out peforms the model created by HUD.

## Data
This project utilizes the data set 05b_analysis_file_update.csv and data dictionary HUD TO3 - 05b Analysis File - Data - Dictionary.csv. These two data sets contain information about the locacl market factors and factors about homelessness. The link to this data source is https://www.huduser.gov/portal/sites/default/files/pdf/Market-Predictors-of-Homelessness.pdf .

## Data Preparation
The data was prepped by  doing a quality check to ensure that the data was suitable to work with. We removed data that was not needed or viable for the project, we also included new derivated varaibles such as converting demographic factors into percents so that the data is easier to work with. The file that does the data prep is: https://github.com/supreetsandhu/Homelessness/blob/main/DATA_3320_Homelessness_Data_Preparation.ipynb . The clean data can found in this repository under homeless_data_prep(1).cvs

## Data Analysis
The data was analyzed by using the lasso and ridge approach of regression.  The lasso and ridge are both a type of regression. The lasso appaorach finds the parameters in the linear model by minimizing a penalized squared error. The ridge approach is used to a type of regression finds the parameters in the linear model by minimizing a penalized squared error. We also used XGboost which is a type of regression. We used the xgBoost to create a tree that uses the best parameters and variables from the dataframe. We also did an extra step where we included the federal funding for each state and included that data in our modeling.
