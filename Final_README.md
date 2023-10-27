
# Capstone-Project-Bike-Sharing-Demand-Prediction-

Predicting the optimal number of bikes needed at any specific moment and day is a crucial and intricate business challenge. Striking the right balance is of paramount importance too few bikes can lead to resource inefficiencies, including maintenance costs and the need for parking and security infrastructure, while an excess of bikes can result in financial losses. These losses encompass immediate revenue reduction due to a limited customer base and potential long-term impacts, such as the erosion of customer trust and loyalty.

Predicting bike sharing demand can help bike sharing companies to allocate bikes better and ensure a more sufficient circulation of bikes for customers

Hence, it is imperative for bike rental enterprises to possess a robust demand estimation mechanism. This mechanism equips them to operate efficiently, maximize resource utilization, and ensure a seamless experience for their customers. Accurate demand forecasts are essential for informed decision-making and the overall success of bike-sharing businesses.My project is about making a predictive model which can help in predicting bike count required at each hour.


## Problem Statement

Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.
## Data Overview

The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.

Attribute Information: 

1)Date : year-month-day

2)Rented Bike count - Count of bikes rented at each hour

3)Hour - Hour of he day

4)Temperature-Temperature in Celsius

5)Humidity - %

6)Windspeed - m/s

7)Visibility - 10m

8)Dew point temperature - Celsius

6)Solar radiation - MJ/m2

7)Rainfall - mm

8)Snowfall - cm

9)Seasons - Winter, Spring, Summer, Autumn

10)Holiday - Holiday/No holiday

11)Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)
## Approach
The following steps were followed in the project:

Data Preprocessing: The dataset was preprocessed and cleaned to handle missing values, outliers, and any inconsistencies in the data.

Data Split: The preprocessed data was split into training and test sets on a random state of 0. By using training data we trained our predictive model and we used testing data to evaluate our prediction.

Model Training:The models were trained using the training data, and their performances were evaluated using various metrics.

Model Evaluation: The performance of the trained models was evaluated using metrics such as mean absolute error, root mean squared error, and R-squared. The model that performed the best on the test data was selected.

Feature Importance: Studies were conducted to understand the impact of individual features on the model's performance. The analysis revealed the significance of temperature, weather conditions, and seasonality features in predicting bike demand.

Model Deployment: The selected model was deployed in a live production setting, where it could make real-time predictions of bike demand. The model's performance was monitored over time to ensure its accuracy and usefulness.
## Models Used
For modeling we tried various regression models such as- 
1)Linear Regression

2)Lasso Regression

3)Ridge Regression

4)Random Forest

5)Gradient Boosting

All these models were fine tuned using a grid search method with repeated cross-validation (CV) to ﬁnd the best hyperparameters. 
We also found out Feature importance so that we get to know about the features which are highly important.
## Results
The model which provides the highest R2 values and lowest MSE, RMSE and MAE is the best one.And this problem can be solved using this model.
## Outputs


![Capture](https://github.com/ady909/Seoul-Bike-Sharing-Demand-Prediction/assets/57126736/6e6e5151-7a35-4970-a367-9ed45d63d90c)

![Capture1](https://github.com/ady909/Seoul-Bike-Sharing-Demand-Prediction/assets/57126736/9f5fff4e-c3fd-4434-b7dd-95682b54cd22)


## Conclusion
During our analysis, Firstly I cleaned the data and conducted an exploratory data analysis (EDA) on all the features in our dataset. Firstly, I analysed my dependent variable 'Rented Bike count' and applied transformations as per requirement.Then I analysed Independent Variables both numerical and categorical variables. I have done Monovariate and Bivariate analysis on these variables . I also studied the numerical variables, calculated their correlations, and the their relationships with the dependent variable. I also handled multicollinearity issue using VIF. I also applied LableEncoding to numerical varibale by adding an Additional Column .

I employed 5 machine learning algorithms including Linear Regression,Lasso , Ridge, Random Forest and Gradient Boosting . I also performed hyperparameter tuning to enhance the performance of our models.

Some facts based on analysis:

1)Gradient Boosting Regressor model shows promising result with R-squared, Adjusted R2 showed highest value and MSE, RMSE showed lowest value , therefore it can be used to solve this problem.

2)There is a huge demand for bike rents in the summer season while the least bike rents occur in winter.

3)Bike demand is more on clear days than on snowy or rainy days.

4)Temperature range from 22 to 25(°C) has more demand for bike.