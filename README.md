California Housing Price Prediction Using Linear Regression and Regularized Regression Models
Project Overview

This project explores the application of linear regression and regularization techniques for predicting housing prices using the California Housing dataset. The study compares the performance of Ordinary Least Squares (OLS) Linear Regression, Ridge Regression, Lasso Regression, Elastic Net Regression, and Stochastic Gradient Descent (SGD) Regression. Model performance is evaluated using standard regression metrics, and coefficient analysis is conducted to examine the effects of regularization on feature importance.

Objectives

The objectives of this project are to:

Build a baseline Linear Regression model.
Implement Ridge, Lasso, Elastic Net, and SGD Regression models.
Compare the predictive performance of all models.
Analyze coefficient shrinkage across the different regression techniques.
Examine feature selection behaviour in regularized models.
Identify the most suitable model for predicting California housing prices.
Dataset

The project uses the California Housing Dataset, which contains information collected from the 1990 U.S. Census.

Features
MedInc – Median income in the district
HouseAge – Median house age
AveRooms – Average number of rooms
AveBedrms – Average number of bedrooms
Population – District population
AveOccup – Average household occupancy
Latitude – Geographic latitude
Longitude – Geographic longitude
Target Variable
MedHouseVal – Median house value
Technologies Used
Python
NumPy
Pandas
Matplotlib
Scikit-learn
Jupyter Notebook
Machine Learning Models

The following regression models were implemented:

Linear Regression
Ridge Regression
Lasso Regression
Elastic Net Regression
Stochastic Gradient Descent (SGD) Regression
Data Preprocessing

The following preprocessing steps were performed:

Data loading
Train-test split (80% training, 20% testing)
Feature standardization using StandardScaler (for regularized models and SGD)
Model Evaluation

The models were evaluated using:

Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
Coefficient of Determination (R²)

Coefficient comparisons were also performed to assess the impact of regularization on model parameters.

Results Summary

The results showed that all regression models achieved very similar predictive performance. Ridge Regression produced results nearly identical to Ordinary Least Squares, while Lasso and Elastic Net achieved slightly lower prediction errors and marginally higher R² values. The differences, however, were practically insignificant.

The coefficient comparison demonstrated that Ridge, Lasso, and Elastic Net shrank coefficient magnitudes relative to Linear Regression. However, none of the regularized models reduced any coefficient exactly to zero, indicating that no automatic feature selection occurred for the chosen regularization parameters.

Conclusion

Among the evaluated models, Lasso Regression achieved the best overall predictive performance, recording the lowest Mean Squared Error and Root Mean Squared Error while maintaining the highest coefficient of determination (R²), although the improvements over the other models were minimal. The findings suggest that all predictor variables contributed meaningful information to the prediction task, resulting in comparable performance across the different regression techniques.
