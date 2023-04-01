# NBA Champion Predictor

## Overview:

This project aims to predict the NBA champion using the NBA API and machine learning models. In this project, player statistics and team standings data are used to train a random forest classifier model to predict the NBA champion of the current season.

## Summary of Workdone:

Data is collected from the NBA API using the "nba_api" Python package. Then, we merged the team standings and player statistics data into a single dataset. We performed feature engineering and selection, followed by data imputation using the mean value. Then, we split the dataset into training and testing sets. We trained a random forest classifier model on the training set, and evaluated its accuracy using the testing set. Finally, we predicted the champion for the current season using the trained model.

### Data:

Type: API Data

Input: NBA team standings and player statistics

Size: 30 teams with multiple player stats

Instances: 82 games per team per season

#### Preprocessing / Clean up:

We merged the team standings and player statistics data into a single dataset and performed feature engineering by creating new features based on existing ones. Then we used data imputation using the mean value for missing values.

### Problem Formulation:

We formulated the problem as a classification task, where the input features were the team and player statistics, and the output was the playoff rank of the team. We used a random forest classifier model to predict the playoff rank.

### Training:

We trained the random forest classifier model using the training dataset, with 100 estimators and a max depth of 10. We used the accuracy score as the evaluation metric.

### Performance Comparison:

Our model achieved an accuracy score of 0.65 on the testing dataset. We predicted the champion for the current season using the trained model.

### Conclusions:

Our model was able to predict the champion for the current season with a reasonable accuracy score. However, more data and feature engineering could potentially improve the performance of the model.

### Future Work:

Further analysis can be done to determine which features have the most significant impact on the model's performance. Additionally, incorporating data from previous seasons could improve the model's predictions.

## How to reproduce results:

Clone the repository and install the necessary packages. Run the code in the provided Jupyter notebook. The NBA API key is required to run the code.

### Overview of files in repository:

nba_champion_prediction.ipynb: main code for data collection, cleaning, and machine learning model training and testing.
README.md: contains information about the project, data, and instructions for reproducing results.
requirements.txt: list of required packages.
LICENSE: MIT license information.

### Software Setup:

Python 3.7 or higher is required along with the following packages:

numpy
pandas
nba_api
scikit-learn
To install the packages, run "pip install -r requirements.txt" in the terminal.

### Data:

The NBA API provides access to the necessary data for this project. An API key is required, which can be obtained from the official NBA website.

### Training:

The model can be trained by running the code in the provided Jupyter notebook. The trained model will be saved and can be used for future predictions.

### Performance Evaluation:

The model's performance can be evaluated by running the code in the provided Jupyter notebook. The accuracy score will be displayed in the output.

## Citations:

nba_api package: https://github.com/swar/nba_api

NBA website: https://www.nba.com/






