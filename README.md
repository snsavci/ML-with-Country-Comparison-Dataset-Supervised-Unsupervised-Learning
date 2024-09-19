# ML-with-Country-Comparison-Dataset-Supervised-Unsupervised-Learning

#  Project Purpose
This project uses a large dataset to compare countries. In this set, countries' Inflation Rate (%), Population Growth Rate (%), GDP per Capita (in USD) and many more values ​​are given. Comments are made according to the data.

# Data Set
The dataset used consists of 145 rows and 36 columns. Data from 6 countries are given over a 24-year period.

# Variables
The dependent variable (y) is determined as the "Inflation Rate (%)" column, and the independent variables (x) are determined as all rows except the "Inflation Rate (%)" column. 

- Various regression algorithms are tried to find the dependent variable. The regression algorithms used in this project are:

from sklearn.linear_model import LinearRegression, Ridge, Lasso, ElasticNet, BayesianRidge
from sklearn.neighbors import KNeighborsRegressor
from sklearn.tree import DecisionTreeRegressor
from sklearn.ensemble import RandomForestRegressor, GradientBoostingRegressor
from sklearn.svm import SVR
from xgboost import XGBRegressor
from sklearn.model_selection import cross_validate
from sklearn.metrics import r2_score

# Model Choosing
The algorithm that gives the best performance is selected, the hyperparameter is optimized and the selected algorithm is evaluated. In this project, it was decided that the regression model that gives the best performance is Ridge. In the evaluation process, Mean Squared Error and Mean Absolute Error were used in this project.
