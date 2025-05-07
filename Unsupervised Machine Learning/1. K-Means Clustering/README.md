# K-Means Clustering

**K-Means Clustering** is an unsupervised learning algorithm that groups data into $k$ clusters based on feature similarity. The algorithm iteratively assigns each point to the nearest cluster centroid and then updates the centroids based on the mean of the assigned points.

The objective is to minimize the within-cluster sum of squares:

$$
\sum_{i=1}^{k} \sum_{x \in C_i} \|x - \mu_i\|^2
$$

where $C_i$ is the set of points in cluster $i$ and $\mu_i$ is the centroid of cluster $i$.

K-Means works best when clusters are **spherical and equally sized**, and it requires the number of clusters $k$ to be specified in advance. It is sensitive to initial centroid placement, so multiple initializations may be used for robustness.

In this project, we use K-Means to **cluster MLB hitters** based on their offensive profiles, using features such as barrel percentage, exit velocity, launch angle, hard hit rate, strikeout rate, walk rate, and ISO. We then visualize the clusters using **PCA** to reduce the feature space to two dimensions.
