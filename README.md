# Flight_delay_forecast_tech_lab

## Abstract

When flights arrive after the scheduled time, it is considered as a delay, which is primarily caused by many factors. Flight delays are inconvenient for passengers and can result in significant financial losses for both airlines and countries. To address this issue, an organized prediction system is essential for aviation authorities to minimize flight delays. The goal of this project is to create a two-part machine learning system that can accurately predict the arrival delay of a flight in minutes after takeoff using real-time flight and airport data. The first stage of the system is a classifier that predicts if the delay of flight is acceptable or not. And in a second part, a regression model is used to predict the amount of time the flight will be delayed upon arrival.

## Code Walkthrough
This repository contains a Python script and images for a two-part machine learning system that accurately predicts the arrival delay of a flight in minutes after takeoff using real-time flight and airport data.

## Overview

Flight delays are a major issue for passengers, airlines, and states, causing significant financial losses. To address this problem, this project aims to create a prediction system that can minimize flight delays using machine learning. The system consists of two parts: a classifier that predicts if the delay of flight is acceptable or not, and a regression model that predicts the amount of time the flight will be delayed upon arrival.

# How the Code Works
Step 1: [Import the Required Modules](./modules.ipynb). 

Step 2: [Data Preprocessing](./Cleaning_flightdelay_sbhusal.ipynb)

Clean and preprocess the collected data by removing irrelevant features, handling missing data,
and transforming categorical variables into numerical values.

Step 3: [Classifying flights as acceptable delay or not](./classifier_many_models_jan_mf.ipynb)

We have trained 5 classification models (Logistic Regression, Decision Tree, Random Forest, Extra tree classifier, and Gradient Boosting Classifier) to predict if the delay of flight is acceptable or not.

Step 4: [Regression Model](./regression.ipynb)

We have trained three regression models (Linear Regression, Linear SVR, and Decision tree) to predict the amount of time the flight will be delayed upon arrival.

## Result
The flight and airport data were merged, and prepared for training a two-stage machine learning model that predicts flight arrival delays. Due to the vast amount of data and limited computational resources, many features had to be excluded. Out of five different classifier models, the logistic regression and Gradient Booster Classifier performed the best with an F1 score of 0.62 and a recall of 0.62 for delayed flights. Also, an AUC score of 0.67 suggests that the models evaluated here are performing better than random guessing. Overall, the classifier model's performance is decent but could potentially be improved, especially for the unacceptable_delay class. 

On the other hand, all three regression models (Linear Regression, Linear SVR, and Decision Tree) produced an RMSE of approximately 2.5 minutes with an R2 score of 0.72. In conclusion, the flight delay prediction was satisfactory and the machine learning model demonstrated good performance. 


# Future Work
## Integration and Deployment
Integrate the trained classifier and regression models into a unified system that can predict the arrival delay of a flight in real-time. The system should deploy on a cloud platform or a web server for easy access and scalability.

The main goal of this project is to provide aviation authorities with an organized prediction system that can minimize flight delays, resulting in improved convenience for passengers and reduced financial losses for airlines and countries.

# Installation Requirements
## Environment
For convenience, it is advised to use a Linux or macOS development environment, although it has not been verified on Windows. The Anaconda package manager and Python 3 (version >= 3.6.4 recommended) should be utilized for package management. It is also suggested to run the code on Jupyter Notebook or Google Colab.

# Dependencies
When using Google Colab and Anaconda, there is no requirement to install:

- matplotlib, 
- scikit-learn, 
- numpy
- pandas
 
since they are already included in these platforms. However, library like 'us' need to install using pip



