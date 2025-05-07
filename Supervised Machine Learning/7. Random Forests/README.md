# Random Forests

**Random Forests** are an ensemble learning method that builds multiple decision trees and combines their outputs to improve predictive accuracy and reduce overfitting. Each tree is trained on a **bootstrap sample** of the data and considers only a **random subset of features** at each split, which introduces diversity among the trees.

For regression tasks, predictions are made by averaging the outputs of all individual trees:

$$
\hat{y} = \frac{1}{T} \sum_{t=1}^{T} \hat{y}_t
$$

This averaging reduces variance and makes Random Forests more robust than a single decision tree. The model handles nonlinear relationships and feature interactions well, and is generally less prone to overfitting.

In this project, we use Random Forests to **predict an MLB player's WAR**, based on Statcast features like barrel percentage, exit velocity, launch angle, and sprint speed.
