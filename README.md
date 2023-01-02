# NYC-Taxi-Trip-Time-Prediction

Project Name - NYC Taxi Trip Time Prediction

Project Status - Complete

Language Used - Python with Pandas, Numpy, Matplotlib, Seaborn, geopy, SKlearn, XGBoost and SHAP libraries

Dataset Link - https://drive.google.com/file/d/1NbtGu1bsgWTo5HznKD71GijSxMLEfPsW/view?usp=sharing

Problem Statement - To predict the trip duration for the nyc taxi trips from 2016 NYC Yellow Cab trip dataset. The data was originally published by the NYC Taxi and Limousine Commission (TLC). The prediction has to be made using various machine learning models and the best performing models will be used for doing future predictions.

Approach - To explore the data in the dataset and extract useful insights from the dataset based on the insights we will be training various machine learning models on some part of the data and the remaining part of data we will be using for testing the trained machine learning models. For the best performing machine learning models we will try to explain the prediction with the help of one of the model explainability technique - SHAP.

Conclusion -

Following are the metrics for the machine learning model used in this project - 

Linear Regression- 	MSE = 171972.702, RMSE = 414.696, R2 = 0.610, Adjusted R2 = 0.610

Lasso-	MSE = 171973.144, RMSE = 414.696, R2 = 0.610, Adjusted R2 = 0.610

Ridge-	MSE = 171973.143, RMSE = 414.696, R2 = 0.610, Adjusted R2 = 0.610

Elasticnet-	MSE = 171973.159, RMSE = 414.696, R2 = 0.610, Adjusted R2 = 0.610

Polynomial- Features	MSE = 160417.946, RMSE = 400.522, R2 = 0.636, Adjusted R2 = 0.636

Decision Tree-	MSE = 131198.160, RMSE = 362.213, R2 = 0.702, Adjusted R2 = 0.702

Random Forest-	MSE = 131254.235, RMSE = 362.290, R2 = 0.702, Adjusted R2 = 0.702

XG Boost-	MSE = 128167.600, RMSE = 358.005, R2 = 0.717, Adjusted R2 = 0.717

Gradient Boosting-	MSE = 128619.268, RMSE = 358.635, R2 = 0.708, Adjusted R2 = 0.708

XG Boost shows lillte bit improvement than Gradient Boosting also the processing time of XG Boost is much lesser as compared to Gradient Boosting. So, we are considering XG Boost as the winner among all the mentioned ML models for this dataset.

SHAP is used to explain the results of XG Boost regressor. Form the charts plotted through SHAP we infer, distance is the most impacting feature in predicting Trip Duration, which is quite obvious as trip_duration is directly dependent on distance. Pickup_hr is also contributing a fair role in predicting Trip Duration as the traffic condition at different time will decide how much time will it take to complete the trip.

Thank you


