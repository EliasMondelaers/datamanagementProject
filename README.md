# datamanagementProject
-------------------------------
# Movie recommendation prediction
-------------------------------------
## Goal of the project: 
For this project we want to predict (yes or no), whether a movie would be recommended to watch by its audience or not. This model can be used by television chains in order to increase their revenue or view numbers. By first checking if the movie they are playing would be recommended or not, they have a larger probability of showing a movie that their audience wants to see, which can give them a competitive advantage.

## Structure of the project: 
1. Data collection
2. Data exploration using visualization
3. Transformation of the target variable (using vote_average to establish a threshold to convert this continious target variable in to a binary target variable (recommend = 1 --> yes, recommend = 0 --> no)
4. Data cleaning + feature engineering
5. Preparation for modeling (train-test split, standardization, creation of interaction feature,..)
6. Modeling using simple models (decision trees, logistic regression, knn) and using their simplicity to interpret the decision making + model evaluation using accuracy
7. Modeling using black box models (XGBoost, Random Forest), and providing feature importance plots + model evaluation using accuracy
8. Creation of bonus regression model: to see if we could also directly predict the rating.

## How to run the project?

Requirements can be found in requirements.txt

All datasets have to be downloaded.

1. Dataset Merging V2.ipynb, will merge the different kaggle datasets into final.csv, which will be the basis to work.
#### Step 2 and 3 do not have to be performed. The resulting csv files can be used immediately (highest_to_lowest_gross.csv and plot_data.csv)
2. Scraping companies.ipynb, will scrape the top movie production companies in the world and will order them into a dataframe from highest to lowest gross profit.
3. Scraping IMDB data.ipynb, will scrape the movie summary and storyline directly from the website for all the movies in the dataset this take +- 20 hours of time.
4. Data preprocessing and Feature Engineering.ipynb, this will prepare and clean the data to immediately be used for modelling for this notebook, this notebook uses hollywood actors.csv, which is a csv that we freely found on the internet containing the most important actors from hollywood. The notebook will output: df_with_budget.csv : which is the dataframe containing the movies for which budget information is available + the budget column, df_without_budget.csv: which is the dataframe containing all the movies and the budget column is excluded, df_regression.csv: which is the dataframe with target variable vote_average instead of recommend.
5. Modeling.ipynb, will try different models and evaluate them using the accuracy metric for the classification problems and RMSE for the regression problem

## Overview of the results: 


Further discussion of the results can be found in the notebooks.
