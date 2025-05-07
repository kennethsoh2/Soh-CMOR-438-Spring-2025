# DBSCAN

**DBSCAN** (Density-Based Spatial Clustering of Applications with Noise) is an unsupervised clustering algorithm that groups together data points that are closely packed, while labeling points in low-density regions as outliers. Unlike K-Means, it does not require specifying the number of clusters in advance.

Two key parameters govern DBSCAN:
- **`eps`**: the maximum distance between two points to be considered neighbors
- **`min_samples`**: the minimum number of points to form a dense region (core point)

A point is assigned to a cluster if it belongs to the neighborhood of a core point. The algorithm expands clusters from these core points and labels all remaining points as either noise or border points.

DBSCAN is effective at discovering **arbitrary-shaped clusters** and identifying outliers, especially when cluster density varies. However, it is sensitive to the choice of `eps`, which is often chosen using a **k-distance plot**.

In this project, we use DBSCAN to cluster **MLB hitters based on their offensive Statcast profiles**, including barrel percentage, exit velocity, launch angle, hard hit rate, and more. PCA is used to visualize the resulting clusters in two dimensions.
