# Robust_yield_prediction

This Repository consists files of the ML Project - customer life time value on for an auto insurance company, It is an academic project for the PG Program in Data Science & Analytics @ Insofe.

Files :

i.   Train_data.csv    - https://drive.google.com/file/d/1VbgvdYREaVCO2_ItSV63NlfkhLwBNaGa/view?usp=sharing

ii.  Farm_data.csv     - https://drive.google.com/file/d/1gztKNe0sAzPMbwTiZsZAMQzZ5rnafk9C/view?usp=sharing 

iii. weather_data.csv  - https://drive.google.com/file/d/16LuknDa3rUnq1GFg01PWcYLItj-Ug-9t/view?usp=sharing

iv.  test_data.csv     - https://drive.google.com/file/d/1y5wUFSahjUK7hXlo31gQ6PagdJXUajHn/view?usp=sharing

v.   test_weather.csv  - https://drive.google.com/file/d/1yLlygP--PwMdCQTjXR8VVGzlp0i50AcO/view?usp=share_link

Robust Yield Prediction Yield Plan.

Introduction: Robust yield prediction is a critical area of research in agriculture that aims to provide accurate forecasts of crop yields, taking into account various factors such as weather patterns, different properties of farm. Accurate yield predictions are essential for ensuring food security, managing crop prices, and optimizing resource allocation.

Traditionally, yield predictions have been made using statistical models that rely on historical data and assumptions about the relationships between crop yield and environmental factors. However, these models often fail to capture the complex and dynamic nature of agricultural systems, resulting in inaccurate and unreliable predictions.

To address this challenge, recent advances in machine learning, data analytics, and remote sensing technologies have enabled the development of more sophisticated and robust yield prediction models. These models leverage large datasets and advanced algorithms to analyze a wide range of variables and generate accurate predictions of crop yields.

Robust yield prediction has significant implications for agricultural management, including optimizing resource use, reducing waste, and improving sustainability. By providing more accurate forecasts of crop yields, farmers can make informed decisions about planting, harvesting, and resource allocation, ultimately leading to more efficient and profitable agricultural systems.

Problem Description :

The problem at hand involves a new fast food chain that has been rapidly expanding over the past few years. As the company continues to grow, they need to ensure that they can meet the increasing demand for their products. To do this, they are looking to optimize their supply chain and ensure that they do not face any shortages of ingredients that could potentially hinder their ability to deliver to customers on time.

To address this challenge, the company has decided to launch a machine learning competition, in which participants are expected to build a model or a set of models that can predict the output of the food processing farms for the next year. 

Methodlogy:

(I) The First stage is understanding the data. there are several datasets were given 

 Datasets releated to Train
 train_dataset         - (date,farm_id,ingrident_type,yield) columns
 train_weather_dataset - (timestamp,deidentified_location,temp_obs,cloudiness,wind_direction,dew_temp,pressure_sea_level,precipitation,wind_speed) 

 Datastes releated to Test
 test_dataset          - (date,farm_id,ingrident_type,id) columns
 test_weather_dataset  - (timestamp,deidentified_location,temp_obs,cloudiness,wind_direction,dew_temp,pressure_sea_level,precipitation,wind_speed)

 Datasets related to Farm
 farm_dataset          - (farm_id,operations_commencing_year,num_processing_plants,farm_area,farming_company,deidentified_location) columns


(II) The Second stage was the Expolratory Data Analysis and Data Preprcessing. In Explorartory Data Analysis we usally see how our data is with the help of
descriptive statistics or data visualizations in what way we have to do data preprocessing based on the analysis we have done on the EDA we will preprocess the
data. such as merging, subsetting datasets, type casting, handling null values.

(III) Model Building: In this stage, using Statistical Models, Machine Learning Algorithms,Ensemble techniques and time series techniques were used.

(IV) Results and Discussions: • For our data in time series models Holt's winter model were forecasts with less root mean square error 945.06 compared to others,
in Ensemble techniques Gradient Boosting Regressor forecasts well with rmse of 795.86

    Model                     RMSE
    
 Simple linear regresson   : 2191.88
 
 Multi linear regresson    : 881.97
 
 Lasso Regression          : 1461.19
 
 Ridge Regression          : 892.25
 
 Decision Tree Regressor   : 9551.99
 
 Random Forest Regressor   : 1393.65
 
 GradientBoostingRegressor : 795.86

 time series models

 Arimax                    : 946.05
 
 Holt's Winter             : 906.61
 
 Arima                     : 1209.98
 
 SArima                    : 945.06
 
 Auto Arima                : 1253.15


# Gradient Boosting Regressor: 
Gradient Boosting Regressor is a machine learning algorithm that is commonly used for regression problems, where the goal is to predict a continuous numerical value. It is an ensemble learning method that builds a sequence of decision trees, where each tree attempts to correct the errors of the previous tree.

The algorithm starts by fitting a simple model to the data and then adding additional models to the ensemble, with each subsequent model focusing on correcting the errors of the previous models. This iterative process continues until the algorithm achieves the desired level of accuracy or reaches a predetermined stopping criterion.

Gradient Boosting Regressor is a powerful algorithm that has proven to be highly effective in a wide range of applications, including finance, healthcare, and agriculture. In agriculture, this algorithm is often used to predict crop yields based on environmental factors such as weather patterns, soil quality.

By leveraging large datasets and advanced algorithms like Gradient Boosting Regressor, farmers and food supply chain managers can make informed decisions about planting, harvesting, and resource allocation, ultimately leading to more efficient and profitable agricultural systems.

# Holt's Winter:
Holt-Winters, also known as Triple Exponential Smoothing, is a time series forecasting method that is commonly used in business and economics to make short-term predictions about future values of a variable based on historical data.

The Holt-Winters method takes into account three components of a time series: trend, seasonality, and level. Trend represents the overall direction of the series, seasonality represents repeating patterns over a fixed period of time, and level represents the baseline value of the series.

The algorithm applies exponential smoothing to each of these three components separately and combines them to make a forecast. The method is called "triple" exponential smoothing because it involves three exponential smoothing calculations.

Holt-Winters is useful when a time series has both trend and seasonality, making it difficult to make accurate predictions using other methods such as simple moving averages. It is a powerful forecasting tool that can be used in a wide range of applications, from finance and economics to weather forecasting and energy demand prediction many more.


Tools and Technology Stack: • Jupyter notebook • Python

Conclusion: The project has successfully demonstrated the use of Holt's Winter in the development of customer life time value
Forecasting model on a dataset consisting of various parameters related to the obtaining of Yiled. The results were very not so realistic in nature as no one were unable to predict the future accurately. 
