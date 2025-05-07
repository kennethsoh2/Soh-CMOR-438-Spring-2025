# Dimensionality Reduction

**Principal Component Analysis (PCA)** is a dimensionality reduction technique that transforms a set of possibly correlated features into a smaller set of uncorrelated components called principal components. These components are linear combinations of the original features and are ordered by the amount of variance they explain.

PCA works by computing the eigenvectors and eigenvalues of the data's covariance matrix and projecting the data onto the top `k` eigenvectors:

$$
Z = XW
$$

where $X$ is the standardized data matrix, $W$ contains the top `k` eigenvectors, and $Z$ is the transformed data.

PCA is useful for visualizing high-dimensional data, reducing noise, and speeding up downstream algorithms. It assumes that the directions of maximum variance capture the most relevant structure in the data.

In this project, we use PCA to reduce the dimensionality of **MLB hitters' offensive profiles**, using features such as swing rate, zone contact, exit velocity, launch angle, barrel percentage, and hard hit rate. The reduced components are later used for visualization or as inputs to clustering algorithms like K-Means and DBSCAN.
