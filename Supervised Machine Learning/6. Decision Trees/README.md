# Decision Trees

**Decision Trees** are a type of supervised learning model that splits data into subsets based on feature values to make predictions. The model learns a series of decision rules by recursively partitioning the data in a way that minimizes some measure of impurity, such as mean squared error (MSE) for regression tasks.

At each split, the model chooses the feature and threshold that results in the best reduction in error. Predictions are made by traversing the tree from root to leaf and returning the average value of the training samples in the final leaf node.

Decision trees are **nonlinear**, interpretable, and flexible, but they can easily **overfit** if the tree is too deep or if regularization (like max depth or min samples per split) is not applied.

In this project, we use a decision tree to **predict an MLB player's WAR**, using input features such as barrel percentage, launch angle, exit velocity, and sprint speed from Statcast data.
