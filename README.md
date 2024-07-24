# Digital-Green-Crop-Yield-Estimate-Challenge
This project aims to develop a machine learning model to forecast the yield per acre of rice and wheat crops across India. By harnessing historical agricultural data and advanced predictive algorithms, the goal is to provide farmers with actionable insights to enhance crop productivity. 

![image](https://github.com/user-attachments/assets/c9daaffe-79f9-4fb8-a2cc-16a904b8ba07)
Challenge Link: https://zindi.africa/competitions/digital-green-crop-yield-estimate-challenge

## Problem Statement
Smallholder farmers are crucial contributors to global food production, and in India often suffer most from poverty and malnutrition. These farmers face challenges such as limited access to modern agriculture, unpredictable weather, and resource constraints. To tackle this issue, Digital Green collected data via surveys, offering insights into farming practices, environmental conditions, and crop yields.

The objective of this challenge is to create a machine learning solution to predict the crop yield per acre of rice or wheat crops in India. Our goal is to empower these farmers and break the cycle of poverty and malnutrition.

A crop yield model could revolutionise Indian agriculture, and serve as a global model for smallholder farmers. Accurate yield predictions empower smallholder farmers to make informed planting and resource allocation decisions, reducing poverty and malnutrition and improving food security. As climate change intensifies, adaptive farming practices become crucial, making precise yield predictions even more valuable. Solutions developed here can drive sustainable agriculture and ensure a stable food supply for the world's growing population. This challenge offers data scientists and machine learning enthusiasts a unique chance to make a real difference in vulnerable populations' lives while advancing global food security in a concise, impactful way.

## Data Cleaning and Pre-processing
Data cleaning and exploration are crucial steps to ensure the accuracy and reliability of the crop yield predictions. The initial phase involves addressing missing values by employing imputation techniques or removing incomplete records, depending on their impact on the dataset. Outliers are identified and analyzed to determine if they represent valid variations or errors that should be corrected. Exploratory Data Analysis (EDA) is then performed to understand data distributions, relationships between features, and underlying patterns. This comprehensive approach ensures that the data is well-prepared for accurate and robust machine learning modeling.

![image](https://github.com/user-attachments/assets/abb606a6-e0af-4b93-8d0b-64a60e8634cf)


## Feature Engineering

In this project, feature engineering encompasses a range of techniques to enhance model performance. Data scaling is applied to standardize feature values and improve model convergence. New features, such as date and time components, are created to capture temporal patterns, while time durations between different processes are calculated to provide additional context. Clustering and grouping are used to identify patterns and segment data effectively, and correlation analysis helps in understanding relationships between features. One-hot encoding is employed to handle categorical variables, ensuring the model can effectively process and learn from all available information.
![image](https://github.com/user-attachments/assets/6ce497a3-c4cd-4073-81fc-7264f7e55409)


## Model Building Process
The model-building journey for this project began with the creation of a Minimum Viable Product (MVP) using Pycaret to establish a baseline. Following this, several machine learning algorithms were explored, including Random Forest, LightGBM, XGBoost, CatBoost, and K-Nearest Neighbors (KNN). Hyperparameter tuning was performed to optimize each model's performance. Subsequently, an ensemble approach was applied to combine the strengths of various models. After thorough evaluation, CatBoost emerged as the best-performing model, demonstrating superior accuracy and robustness for predicting crop yields.
![image](https://github.com/user-attachments/assets/85bd663f-449c-41bf-9af8-c866adb26efe)



## Models Comparison
In evaluating the performance of our models, RMSE (Root Mean Squared Error) is used as the key criterion. The RMSE values for the models tested are as follows: Pycaret provided a baseline RMSE, while Random Forest, LightGBM, XGBoost, CatBoost, and K-Nearest Neighbors (KNN) each demonstrated varying levels of performance. Hyperparameter tuning and ensemble methods were applied to optimize these models. Ultimately, CatBoost achieved the lowest RMSE, indicating it was the most accurate and effective model for predicting crop yields.

![image](https://github.com/user-attachments/assets/cf68b3a3-4d45-4a50-b122-1c85142ba5e7)


## Hyperparameter Tuning

The following images illustrate the various hyperparameters we explored and their corresponding results. These visualizations showcase the range of parameters tested for each model and the impact of these adjustments on performance metrics. By analyzing these results, we identified the optimal hyperparameters that contributed to the best-performing model, CatBoost, which ultimately delivered the most accurate predictions for crop yields.
![image](https://github.com/user-attachments/assets/e7fd1134-1460-4306-a6f6-31faaa806770)
![image](https://github.com/user-attachments/assets/b8a769f5-f4bd-43e8-87a8-898793eef583)



## Best Model Insights

The model analysis revealed several key insights. 
- Significant weight was given to the sqrt_acre feature, which influenced predictions substantially. However, missing values in other features led to inaccuracies, with predictions largely driven by the sqrt_acre pattern.
- Major deviations and variance in features such as TransIrriCost, 1TDUrea, and CropCultLand contributed to prediction inaccuracies.
-  Additionally, while the model struggled with predicting outlier yield values, it exhibited relatively better accuracy for lower yield predictions, highlighting areas for potential improvement.
![image](https://github.com/user-attachments/assets/c7c05911-e2ad-4c62-949c-cbd58678d473)
![image](https://github.com/user-attachments/assets/3057bd7e-ea42-49ac-8798-cd1fe0ec8e0a)







