# K-Nearest Neighbors

**K-Nearest Neighbors (KNN)** is a non-parametric, instance-based learning algorithm used for both classification and regression tasks. Instead of learning explicit model parameters, KNN makes predictions based on the outcomes of the $k$ most similar data points in the training set.

In regression, the predicted value is typically the **average of the target values** of the $k$ nearest neighbors:

$$
\hat{y} = \frac{1}{k} \sum_{i=1}^{k} y_i
$$

NN relies on a **distance metric** (such as Euclidean distance) to measure similarity between points. Because it stores the entire training set, it is considered a lazy learner and can be computationally expensive for large datasets.

This model works best when the relationship between features and the target is **locally smooth**, and when features are appropriately scaled.

In this project, we use KNN to **predict an MLB player's wRC+**, a continuous measure of offensive performance, using Statcast-style features like barrel percentage, exit velocity, and launch angle.
