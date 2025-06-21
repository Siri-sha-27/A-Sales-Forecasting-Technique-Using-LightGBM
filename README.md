# A LightGBM-Driven Framework for E-Commerce Sales Forecasting and Real-Time Inventory Optimization

Problem Statement:
Conventional forecasting techniques often fail to accurately model the dynamic and non-linear patterns of consumer purchasing behavior, leading to inefficiencies in inventory planning.
Key Objective:
To develop an intelligent, machine learning-based forecasting system that can accurately predict item-level sales and support data-driven inventory optimization in retail environments.
Key Approach:
A comparative evaluation of three powerful ensemble learning algorithms—Random Forest, XGBoost, and LightGBM—was conducted. The goal was to identify the model that delivers the best predictive performance on real-world sales data.
Outcome:
Among all the models tested, LightGBM achieved the lowest Root Mean Squared Error (RMSE), making it the most effective model for deployment in a production setting.
 This result demonstrates LightGBM's ability to capture both seasonality and demand fluctuations with high accuracy.
## Pre -Processing and Feature engineering
1. Data collection:
   Data Collection & Preprocessing
Dataset Used: Historical sales data from an e-commerce platform (1C Company).
Granularity: Daily transactional records aggregated monthly using date_block_num.
Initial Cleaning:
Removed negative prices and sales.
Converted date to datetime format.
Extracted Month, Year, Day, and Weekday features.
2. Feature Engineering
   Lag Features: 
Rolling Statistics
Temporal Indicators
Price and Demand Signals
These engineered features help the model understand seasonal trends, price effects, and recent demand dynamics more effectively.
## Model building and focus:
Comparative Model Training
Implemented and compared three ensemble learning models:
Random Forest Regressor
 XGBoost Regressor
 LightGBM Regressor (Primary model in our study)
# Why LightGBM:
Optimized for large-scale data.
Fast training speed using histogram-based learning.
Leaf-wise tree growth for better accuracy.
Low memory usage – ideal for high-dimensional retail features.
LightGBM Configuration:
Tuned hyperparameters using GridSearchCV:
n_estimators, max_depth, learning_rate
subsample, colsample_bytree
Achieved optimal balance between bias and variance.
## Techinque used:
1.Gradient Boosting Framework
2.Leaf-wise Tree Growth
3.Histogram-based Learning
4.Key Tuned Parameters
5.Cross-Validation

## Analysis of the results:
![image](https://github.com/user-attachments/assets/bdfecbde-879e-431a-96f5-4d1b97541341)

![image](https://github.com/user-attachments/assets/2f070514-e6e2-4968-82f1-d5c46f5b5500)


![image](https://github.com/user-attachments/assets/4f759927-bc4c-45d5-b6e9-729cbc4b684b)

## Conclusion:
Machine learning models significantly enhance forecasting accuracy in e-commerce, outperforming traditional methods.

Note: Please refer to IEEE format paper for more clear understanding and insights of our project.
