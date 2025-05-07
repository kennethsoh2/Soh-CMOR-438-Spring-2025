# Neural Networks

**Neural Networks** are a class of machine learning models inspired by the structure of the human brain. A basic feedforward neural network consists of an input layer, one or more hidden layers, and an output layer. Each layer applies a weighted transformation followed by a nonlinear activation function.

For binary classification, the output neuron typically uses the **sigmoid activation function**:

$$
\sigma(z) = \frac{1}{1 + e^{-z}}
$$

Weights are updated using **stochastic gradient descent** and **backpropagation**, which computes gradients layer by layer to minimize the binary cross-entropy loss.

Neural networks are especially powerful when the relationship between input features and the target variable is **nonlinear**. However, they require more data and tuning than simpler models like logistic regression.

In this project, we use a feedforward neural network to classify whether an **MLB player had over or under 2.5 WAR** during the 2022 season, based on Statcast features like barrel percentage, exit velocity, launch angle, and sprint speed.
