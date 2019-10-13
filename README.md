# Super-Heroes

Problem Statement:

The objective of the problem is to identify whether a super hero is a human or not based on the several characteristics or factors.

Data Sources:

It contains two files. namely heroes_information.csv(which contains heroes information) super_hero_powers.csv(contains powers of super heroes) 

Data Preprocessing and Preparation:

Started with understanding the data and performing simple sanity checks. Filtered out the rows which are having null/unknown(-) values in Race column. Then proceed with performing missing value and outlier analysis. Identified that few attributes/columns such as weight, publisher consists of missing values. Imputed those missing values using imputation techniques such as median and model based imputation. 

Then performed exploratory data analysis on dataset which includes uni-variate and bi variate analysis. This is to understand more about the data, relationship between the attributes and deriving useful insights from data. Few notable techniques performed in EDA were data aggregation, correlation analysis, exploratory plots etc., Then proceeded with data preparation which includes feature engineering and joining the tables. Derived the target variable by flagging human as 1 and other values as 0. Created the dummy variables for categorical attributes using one hot encoding techniques as a part of feature engineering process. Joined the different data sources information together in order to bring all features into one dataset. 

Feature Selection:

Removed few variables like id/name and variables which are having high percentage of missing values.

Model Building

Once the data preparation and feature selection completed, built the ML model. In this step, first we divided the data into train and test using stratified sampling. Then applied different classification algorithms such as logistic regression and random forest. 

Model Evaluation:

Evaluated the model on unseen test data and obtained the 75 % accuracy. Used to area under ROC curve to understand how model is performing. AUC of the random forest model on the unseen data is 82% which shows model is having high discriminative ability

