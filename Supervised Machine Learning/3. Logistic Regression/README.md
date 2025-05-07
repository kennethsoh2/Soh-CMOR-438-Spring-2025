# Logistic Regression

**Logistic Regression** is a classification model that outputs probabilities between 0 and 1. Like linear regression, it computes a weighted sum of the inputs, but it then passes this value through a sigmoid function to map it into the [0, 1] range. This makes it suitable for binary classification tasks.

The logistic regression model is defined as:

$$
P(y = 1 \mid \mathbf{x}) = \frac{1}{1 + e^{-\mathbf{x}^\top \boldsymbol{\beta}}}
$$

We estimate the weights $\boldsymbol{\beta}$ using **gradient descent**, which iteratively updates the model based on the binary cross-entropy loss. This process continues for a fixed number of epochs or until convergence.

Logistic regression is most effective when the data is **linearly separable**. It differs from the perceptron by using soft probabilities instead of hard thresholds, which allows for more stable updates and probabilistic interpretation.

In our case, we apply logistic regression to MLB player data. For example, we use Statcast features like barrel percentage, exit velocity, and launch angle to predict whether a player is an All-Star (1) or not (0). The model outputs the probability that each player qualifies as an All-Star based on these performance indicators.
