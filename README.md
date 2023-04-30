# NBA Champion Predictor

## Overview:

This project aims to predict the NBA champion using the NBA API and machine learning models. In this project, player statistics and team standings data are used to train linear regression and random forest classifier models to predict the NBA champion of the current season.

## Summary of Workdone:

Data is collected from the NBA API using the "nba_api" Python package. Then, we merged the team standings and player statistics data into a single dataset. We performed feature engineering and selection, followed by data imputation using the mean value. Then, we split the dataset into training and testing sets for model evaluation.
Two machine learning models, a Linear Regression model and a Random Forest Classifier model, were trained on the training dataset.
                  
### Data:

Type: API Data

Input: NBA team standings and player statistics

Size: 30 teams with multiple player stats

Instances: 82 games per team per season

#### Preprocessing / Clean up:

We merged the team standings and player statistics data into a single dataset and performed feature engineering by creating new features based on existing ones. Then we used data imputation using the mean value for missing values.

### Problem Formulation:

We formulated the problem using two approaches: a regression task and a classification task. For the regression task, the input features were the team and player statistics, and the output was the winning percentage of the team. We used a linear regression model to predict the winning percentage. For the classification task, the input features were the team and player statistics, and the output was the playoff rank of the team. We used a random forest classifier model to predict the playoff rank.

### Training:

We trained the linear regression model and the random forest classifier model using the training dataset. The random forest classifier model was trained with 100 estimators and a max depth of 10. We used the R2 score for evaluating the linear regression model and the accuracy score for evaluating the random forest classifier model.

### Performance Comparison:

The linear regression model achieved an R2 score of 0.5188 on the testing dataset, while the random forest classifier model achieved an accuracy score of 0.23 on the testing dataset. We predicted the champion for the current season using both trained models.


### Conclusions:

Both models were able to predict the champion for the current season with reasonable accuracy scores. However, more data and feature engineering could potentially improve the performance of the models.

### Future Work:

Further analysis can be done to determine which features have the most significant impact on the models' performance. Additionally, incorporating data from previous seasons could improve the models' predictions. Experimenting with other machine learning models may also yield better results.
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






