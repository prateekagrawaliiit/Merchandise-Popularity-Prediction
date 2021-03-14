# MERCHANDISE POPULARITY PREDICTION (Multiclass Classification)

## [Leaderboard Position](https://www.machinehack.com/hackathons/merchandise_popularity_prediction_challenge/leaderboard) : 33/637 (Top 5.1%) 

Objective :

Big Brands spend a significant amount on popularizing a product. Nevertheless, their efforts go in vain while establishing the merchandise in the hyperlocal market. Based on different geographical conditions same attributes can communicate a piece of much different information about the customer. Hence, insights this is a must for any brand owner.

In this competition, we have brought the data gathered from one of the top apparel brands in India. Provided the details concerning category, score, and presence in the store, participants are challenged to predict the popularity level of the merchandise. 

The popularity class decides how popular the product is given the attributes which a store owner can control to make it happen.

 
### Dataset Description:
Train.csv - 18208 rows x 12 columns (Includes popularity Column as Target variable)
Test.csv - 12140 rows x 11 columns

Steps :

- Exploratory Data Analysis - There are a few outliers in certain columns
- Feature Engineering - Generated new features using the agg of catorical columns with the continuous ones.
- Model Selection - Experimented with different models and finally used Catboost,XGBoost and LightGBM
- Final Model - Used an emsembled on the above three models with a weighted average based on their public leaderboard scores.
- Post-Processing - Identified that certain rows in test are present in train and can be directly used.
