# Perceptron
# 🧠 Perceptron Classifier (Custom Implementation)

## 📌 Overview

The Perceptron is a simple yet foundational supervised learning algorithm used for **binary classification**. It models a linear decision boundary by iteratively adjusting weights based on misclassified training examples. As the building block for more complex neural networks, the perceptron introduces key ideas such as activation functions, weight updates, and convergence based on labeled feedback.

In this project, the Perceptron was applied to predict whether an MLB player qualifies as an All-Star based on Statcast-style hitting metrics (e.g., Barrel%, Exit Velocity, and HardHit%). This provides insight into how well linear boundaries can separate high-performing hitters from the rest.

---

## ⚙️ Core Implementation Details

The `Perceptron` class contains three main methods:

- `fit(X, y)`: Trains the model by updating weights using the Perceptron learning rule.
- `predict(X)`: Returns predictions (`0` or `1`) using the sign of the weighted sum.
- `score(X, y)`: Calculates accuracy by comparing predictions to true labels.

The activation function is a simple step function:

