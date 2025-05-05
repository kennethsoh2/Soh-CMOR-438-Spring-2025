# Linear Regression
# Linear Regression (Custom Implementation)

## Overview

Linear Regression is a foundational supervised learning algorithm used to model the relationship between a set of input features and a continuous target variable. It assumes a linear relationship of the form:

    ŷ = w₁x₁ + w₂x₂ + ... + wₙxₙ + b

where ŷ is the predicted output, wᵢ are the learned weights, and b is the bias term. The model is trained to minimize the mean squared error (MSE) between predictions and actual target values.

In this project, linear regression was used to predict a hitter’s wRC+ using Statcast-style metrics such as Exit Velocity, Barrel%, and Launch Angle. This served as a baseline model for offensive performance prediction.

## Core Implementation Details

The `LinearRegressionNeuron` class is a custom single-layer model that implements basic gradient descent. It includes the following methods:

- `fit(X, y)`: Trains the model using gradient descent to minimize squared error.
- `predict(X)`: Returns continuous-valued predictions using the learned weights.
- `score(X, y)`: Computes the R² score to evaluate the proportion of variance explained.

The loss function minimized is the Mean Squared Error (MSE):

    MSE = (1/n) * Σ(yᵢ - ŷᵢ)²

Weight updates during training follow:

    w ← w - α * ∂MSE/∂w
    b ← b - α * ∂MSE/∂b

where α is the learning rate.

## Training Procedure

- Input features were standardized prior to training.
- Weights and bias are initialized to small random values.
- At each iteration, gradients are computed and parameters are updated until convergence or a maximum number of epochs is reached.

## Project Application

- Task: Predict hitter wRC+ (continuous target).
- Dataset: 2022 MLB hitters with ≥ 100 plate appearances.
- Features: Barrel%, Exit Velocity, Launch Angle, etc.
- Results: The linear model produced a reasonable R² score and helped highlight which features (like Barrel%) contribute most linearly to wRC+. However, it also revealed limitations in modeling nonlinear patterns, motivating the use of more complex models like decision trees and neural networks.