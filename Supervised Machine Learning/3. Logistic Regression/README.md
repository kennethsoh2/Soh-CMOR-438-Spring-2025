# Logistic Regression

**Logistic Regression** is a classification model that outputs probabilities between 0 and 1. Like linear regression, it computes a weighted sum of input features, but it then applies the sigmoid function to map that value into a probability range.

The model is defined as:

$$
P(y = 1 \mid \mathbf{x}) = \frac{1}{1 + e^{-\mathbf{x}^\top \boldsymbol{w}}}
$$

The weights are estimated using **gradient descent** by minimizing the **binary cross-entropy loss** between predicted probabilities and actual labels.

Logistic regression is best suited for **binary classification problems**, especially when the classes are linearly separable or nearly so. Unlike the perceptron, it outputs soft probabilities rather than hard class boundaries, making it more stable for noisy data.

In this project, we use logistic regression to predict whether an **MLB player had over 1 WAR** in the 2022 season, based on features such as barrel percentage, exit velocity, and launch angle from Statcast data.

