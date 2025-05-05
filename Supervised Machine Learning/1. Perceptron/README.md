# Perceptron

## Overview

The Perceptron is a simple yet foundational supervised learning algorithm used for **binary classification**. It models a linear decision boundary by iteratively adjusting weights based on misclassified training examples. As the building block for more complex neural networks, the perceptron introduces key ideas such as activation functions, weight updates, and convergence based on labeled feedback.

In this project, the Perceptron was applied to predict whether an MLB player qualifies as an All-Star based on Statcast-style hitting metrics (e.g., Barrel%, Exit Velocity, and HardHit%). This provides insight into how well linear boundaries can separate high-performing hitters from the rest.

---

## Core Implementation Details

The `Perceptron` class contains three main methods:

- `fit(X, y)`: Trains the model by updating weights using the Perceptron learning rule.
- `predict(X)`: Returns predictions (`0` or `1`) using the sign of the weighted sum.
- `score(X, y)`: Calculates accuracy by comparing predictions to true labels.

The activation function is a simple step function:
ŷ = 1 if w · x + b ≥ 0
0 otherwise

Weight updates occur according to the rule:
w ← w + α(y - ŷ)x

## Training Procedure

- All features are normalized prior to training.
- A learning rate (α) is used to scale the magnitude of updates.
- The model iterates over the training data multiple times (epochs), updating only on errors.

## Project Application

- **Task**: Predict All-Star status (binary classification).
- **Dataset**: Cleaned MLB Statcast data from 2022.
- **Features**: Barrel%, Exit Velocity (EV), Launch Angle (LA), and more.
- **Outcome**: The perceptron reached moderate performance, highlighting that All-Star classification may not be linearly separable. This benchmark served as a useful baseline for comparison with more complex models like logistic regression and neural networks.