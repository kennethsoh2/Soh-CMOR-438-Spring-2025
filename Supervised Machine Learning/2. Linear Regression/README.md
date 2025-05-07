# Linear Regression

**Linear Regression** is a foundational regression algorithm that models the relationship between input features and a continuous target variable. It assumes a linear relationship, meaning the target is predicted as a weighted sum of the input features.

The model is defined as:

$$
\hat{y} = \mathbf{x}^\top \boldsymbol{\beta} + \beta_0
$$

where $\boldsymbol{\beta}$ are the learned coefficients and $\beta_0$ is the intercept. These parameters are typically estimated using **gradient descent** or **ordinary least squares (OLS)** to minimize the mean squared error (MSE) between predictions and actual values.

Linear regression is most effective when the target variable has a **linear dependence** on the features and the residuals are homoscedastic and normally distributed.

In this notebook, we use linear regression to **predict a player's WAR** based on features like barrel percentage, exit velocity, launch angle, and sprint speed from MLB Statcast data.

