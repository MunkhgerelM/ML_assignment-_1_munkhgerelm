# Regression Model Comparison 
This assignment compares the performance of different regression models for a specific regression problem. The goal is to predict a target variable based on input features using various regression techniques.

The family of model is given as: `f(x, theta) = theta_0 + theta_1 * x_1 + theta_2 * x_2 + theta_3 * cos(x_1) + theta_4 * x_2 * x_2 + theta_5 * tanh(x_1) ` to fit the data (File: **data.npz**). 

## Problem Description
The regression problem involves predicting a continuous target variable based on multiple input features. The dataset used in this analysis contains both training and test datasets, allowing for model evaluation on unseen data.
Models Evaluated

1.	Linear Regression: This baseline model uses a linear relationship between the input features and the target variable.

2.	Lasso Regression: Lasso regression adds L1 regularization to the linear regression model, promoting sparsity and potentially aiding in feature selection.

3.	Polynomial Regression: This model extends linear regression by incorporating polynomial features, allowing for more complex relationships between the features and the target variable.


## Evaluation Metric
The performance of each model is evaluated using the mean squared error (MSE) on both the training and test datasets. A lower MSE indicates better model performance.
Results are the following:
### Linear Regression:
*	MSE on Test Data: 0.003294
*	MSE on Train Data: 0.003227
### Lasso Regression:
*	MSE on Test Data: 0.9668
*	MSE on Train Data 1.0000
### Polynomial Regression:
*	MSE on Test Data: 1.47446
*	MSE on Train Data: 1.38041

### Statistical Comparison
A paired t-test was conducted to compare the performance of linear regression and polynomial regression models. There is a significant difference in performance between linear regression and polynomial regression. (p-value > 0.05), indicating that Linear model performs better than polynomial regression model. 

## Conclusion
Based on the MSE comparison and statistical analysis, the linear regression shows better performance for this regression problem than and polynomial regression model.




