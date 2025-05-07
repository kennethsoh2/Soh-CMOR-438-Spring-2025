# Perceptron

**Perceptron** is one of the earliest and simplest classification algorithms. It attempts to find a linear decision boundary that separates two classes by updating weights based on prediction errors. The model uses a hard threshold: if the weighted sum of inputs exceeds zero, it predicts class 1; otherwise, it predicts class 0.

The perceptron model is defined as:

$$
\hat{y} = 
\begin{cases}
1 & \text{if } \mathbf{x}^\top \boldsymbol{w} + b \geq 0 \\
0 & \text{otherwise}
\end{cases}
$$

Weights $\boldsymbol{w}$ and bias $b$ are updated through the perceptron learning rule each time the model misclassifies a training example.

The perceptron works best on **linearly separable** datasets and does not produce probabilistic outputs. It is a deterministic, mistake-driven learner that converges only if a perfect linear separator exists.

In our implementation, we apply the perceptron to predict binary outcomes in an MLB context — for example, determining whether a player had an above-average wRC+ based on features like exit velocity, launch angle, and hard hit rate.
