# AirBnb-Price-Prediction-with-Machine-Learning
Airbnb price prediction using machine learning and EDA on it.

![image](https://user-images.githubusercontent.com/109715598/216969316-13e17f89-5752-428c-bd74-af007763c235.png)


## Introduction 
- Airbnb was founded in 2008 as a platform enabling locals to list their homes for short term rental and travelers to have a lodging option alternative to hotels.
- Airbnb net worth as of January 13, 2023 is $64.48B.
- This Dataset is collected in year 2019.
- Along with homes for rent, Airbnb.com allows its users to search through “Experiences”, which include pre-arranged multi destination trips, “Restaurants,” and         recently even “Animals,” which stands for experiences where travelers can meet and interact with animals local to their travel destination (e.g., Zoo visit).

## Context
- The data was obtained from Kaggle :https://www.kaggle.com/datasets/arianazmoudeh/airbnbopendata/code.
- Since 2008, guests and hosts have used Airbnb to travel in a more unique, personalized way. As part of the Airbnb Inside initiative, this dataset describes the         listing activity of homestays in New York City

## Problem Statement 
- What are the factors and features of a listing that make an Airbnb listing more Expensive.
- Problem 1: Host identity verification affect the Airbnb pricing?
- Problem 2: Reviews for AirBnb which effect the Airbnb?
- Problem 3: What is the range of prices in Airbnb?
- Problem 4: Availability according to months.

## Questionnaire 
1) How many days do the owners of the house receive the guest in their house throughout the year.
2) Which neighbourhood do you give the highest ratings.
3) What is the range of prices ?
4) Host identity verified effect on price ?
5) Relationship with neighbourhood group and the price ?
6) What are the proportions of room types?
7) Most Construction year ?

## Dataset:
- This dataset consist of Records:102599 and Features:26

## Python Libraries used in Project
- import numpy as np
- import pandas as pd
- import matplotlib.pyplot as plt
- import seaborn as sns
- import warnings
  warnings.filterwarnings('ignore')

## Data Preparation/Cleaning
1) As the dataset from kaggle was not very suitable for data analysis, we had to change the format of some data in the dataset. We also had to do separate data preparation for exploratory analysis and machine learning.
2) Some of our data preparation were:
3) Convert price of listings from strings to floats and also remove the '$' sign.
4) Change NaN values to the integer 0.
5) Cleaning the textual data into a form that would be suitable for Python's Jupyter Notebook.
6) Encoding the categorical variables so that it can be fit into the regression models later.
7) Separating the data into Predicted and Target variables.
8) Separating the data into training and testing sets (Training Sets: Testing Sets = 70% : 30%)

## Use of Regressor in the Machine Learning Models.
Regression is a supervised machine learning technique which is used to predict Continuous values. The ultimate goal of the regression algorithm is to plot a best-fit line or a curve between the data.
Machine Learning Regression is a technique for investigating the relationship between independent variables or features and a dependent variable or outcome. It's used as a method for predictive modelling in machine learning, in which an algorithm is used to predict continuous outcomes.
There is no categorical Values in the dataset so, will not use the Classifiers in the Machine Learning Models.
That's Why we use Regressor Model in this Dataset.

## ML Model Used in project:
1) Decision Tree Regressor = 99%
2) Random Forest Regressor = 99%
3) Linear Regression = 98%%
4) XGBoost Regressor = 99%

## Conclusion
From all the analysis done above, we can confidently answer our initial question of the factors that make a listing more expensive. An aspiring Airbnb host, if investing on a new properties, should focus on the following factors to maximize the price of his listing. Additionally a traveller who wants to pay the lowest - possible price for a listing might want to avoid having these features in his prospective housing

1) Entire properties listed instead of just a single room fetch the highest prices.
2) Apartment and landed house tend to be the most expensive and the most abundant properties in Airbnb.
3) The more bedrooms a property has, the higher its price. The highest prices are fetched by 6 room properties.
4) There are plenty of listings in Belltown or West Queen Anne and they tend to be expensive.
5) Words like: view, modern & walk all frequently appear in the summary of the more expensive listing.
6)Ammenities such as: Washer, Dryer, Heating, Wireless Internet, Smoke Detector, Free Parking, Kid Friendly, TV, HotTub/Sauna/Pool, Gyms and Elevators are all common among the more expensive listings.
7)The reviews a listing gets (quality or quantity) does not have much of an impact in its price.

