# Product-Sales-Outlet-at-BigMart-Datawarehouse<br>


### Project Description<br>
The data scientists at BigMart have collected 2013 sales data for 1559 products across 10 stores in different cities. Also, certain attributes of each product and store have been defined. The aim of this data science project is to build a predictive model and find out the sales of each product at a particular store.
Using this model, BigMart will try to understand the properties of products and stores which play a key role in increasing sales.
 The data has missing values as some stores do not report all the data due to technical glitches. Hence, it will be required to treat them accordingly.


### We will handle this problem in a structured way. We will be following the table of content given below.<br>

1). Problem Statement
2). Hypothesis Generation
3). Loading Packages and Data
4). Data Structure and Content
5). Exploratory Data Analysis
6). Univariate Analysis
7). Bivariate Analysis
8). Missing Value Treatment
9). Feature Engineering
10). Encoding Categorical Variables
11). Label Encoding
12). One Hot Encoding
13). PreProcessing Data
14). Modeling
15). Linear Regression
16). Regularized Linear Regression
17). RandomForest
18). XGBoost
19). Summary

### Curriculum For This Project<br>

1). The Business Problem Exploring 
2). The Dataset 
3). Exploratory Data Analysis (eda) - Outliers
4). Exploratory Data Analysis (eda) - Graphs
5). Converting Categorical To Numerical
6). Seperating Training And Test Data
7). Running The Models
8). Hyper Parameter Tuning XGB And GBR
9). Standard Scaling 06m Robust Scaling
10). Final Predictions On The Test Dataset
11). Saving The Final Model

### Link to Download the Dataset<br>

<a href="https://bit.ly/3sVgopt" target="_blank">Download Dataset</a>

### RMSE Scores after training different models on default parameters:<br>

- GradientBoostingRegressor 1081.5751391944918        
- LGBMRegressor 1107.908405729656        
- CatBoost 1120.0096666517916        
- Ridge 1124.6431654694052        
- linear regression 1124.6437648088292        
- RandomForestRegressor 1130.8483158529339        
- XGBRegressor 1189.5514050886934        
- ElasticNet 1257.3462638940737        
- KNeighborsRegressor 1448.803026944895        
- SVR 1596.562744491264        
- SGDRegressor 2510970101894195.0 

### After HyperParameter tuning.<br>

- Results of GradientBoostingRegressor model
    - Best Model with Parameters:  {'max_depth': 2, 'max_features': 'auto', 'n_estimators': 90, 'warm_start': False}
    - Best Score:  -1156914.1730931485
    - RMSE score:  1075.599448258109

- Results of CatBoost model
    - Best Model with Parameters:  {'depth': 4, 'learning_rate': 0.05, 'n_estimators': 100, 'reg_lambda': 0.2}
    - Best Score:  -1151683.0287196394
    - RMSE score:  1073.164958764327

- Results of Ridge model
    - Best Model with Parameters:  {'max_iter': 1200, 'solver': 'cholesky', 'tol': 0.1}
    - Best Score:  -1267971.2134231322
    - RMSE score:  1126.0422787014404

- Results of LGBMRegressor model
    - Best Model with Parameters:  {'max_depth': 2, 'n_estimators': 100, 'reg_alpha': 0.25, 'reg_lambda': 0}
    - Best Score:  -1150036.0188730017
    - RMSE score:  1072.3973232309943

GradientBoostingRegressor,  LGBMRegressor,  CatBoost  all 3 are performing equally good on cross validation on training set.

### Evaluating Performance on test set.<br>

- RMSE score of GBR model on test set:  1733.65473483868
- RMSE score of LGBM model on test set:  1737.7360427637957
- RMSE score of CatBoost model on test set:  1732.9670316396723

### Best Performers.<br>

GradientBoostingRegressor   and   CatBoost models are performing best.

