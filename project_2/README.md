# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: AMES Housing Data and Kaggle Challenge

### Problem Statement 


**Predicting the sale prices of residential housing in Ames, using advanced regression techniques and machine learning algorithms.**

---

### Executive Summary


This project investigates factors that influence decision-making calculus of potential home buyers and how various attributes of a property impacts its sales price. The aim of the project is to build a housing sale price prediction model using the most important attributes (or features) of the house. 

To achieve the objective of predicting sales prices of residential housing in Ames, we were provided with two different data sets: train and test. The Train Dataset comprised of observations of 2051 different properties (rows) and 81 different characteristics or features (columns) of the property. The columns comprised of 22 nominal, 21 ordinal and 38 continuous (numerical) continuous
variables. The two other columns were the identification columns. On the other hand, the Training data set provided the context to build a model for predicting sale prices. The test data set, for which sale prices were to be predicted, comprised of 879 observations (properties) and 80 features or characteristics. The test data set, unlike the training data set, does not include sale price as a variable since this was the value to be predicted.

---

### Datasets 


The project uses the following datasets. 

- [Housing Train Dataset](./datasets/train.csv)
- [Hosuing Test Dataset](./datasets/test.csv)

These data give information about different features of the residential housing units in AMES, Iowa. The detailed data dictionary can be accessed at 

---

### Data Dictionary

The detailed data dictionary for this project can be accessed at - 
[data description](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt).

---

### Conclusion and Recommendations

I ran correlation on my training data set to find out which variables are strongly correlated with the dependent variable, the sale price. Variables such as overall quality, ground living area, garage area, garage cars, total basement area were found to be highly correlated with sales price. The correlation was also strong between some of the independent variables. For example, garage
cars and garage area were significantly correlated. To eliminate multi-collinearity, one of either variables had to be dropped while building the prediction model.

After dividing the training set into Train and Validation set, several models were fitted on the Train and tested on the Validation set to find the best model. The best model is the one which is able to predict the sale price most efficiently and precisely. I ran Linear Regression, Lasso Regression, Ridge Regression and ElasticNet Regression to find the highest accuracy score (i.e. R-squared value). The ElasticNet regression provided the best R-squared value and the Root Mean Squared error for the validation set slightly improved over the Root Mean Squared error of the Train set. Therefore, Elastic Net Regression is preferred over other methods and is applied to the validation test. ENet coefficients were calculated and the final prediction model was built using 22 variables including both categorical and continuous variables. Eventually, this prediction model was tested on the Housing Test Data set and sale price predictions were made. 

Feature engineering of some of the variables by using higher-order polynomial function is recommended to deal with the issue of overfitting of variables and selecting the most important variables. Some of the features can be combined with others to produce one feature such as total bathrooms could be calculated by weighting and summing up the half and full bathrooms. This approach would automatically eliminate some amount of multi-collinearity among the explanatory variables. 
