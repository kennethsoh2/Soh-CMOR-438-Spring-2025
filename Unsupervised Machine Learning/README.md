# Unsupervised Learning Algorithms

**Unsupervised Machine Learning** explores patterns and structure in data without predefined labels. These methods are especially useful for discovering hidden groups or relationships within player data based solely on statistical similarity.

The main focus in this section is **clustering**, where players are grouped based on how similar they are across a set of features. Unlike classification, these groups are discovered from the data, not assigned in advance.

In this section, we apply the following unsupervised learning techniques to MLB hitter data:

1. **K-Means Clustering** — Groups players with similar offensive Statcast profiles, such as Barrel%, Launch Angle, and Hard Hit%.
2. **DBSCAN** — Identifies dense regions of similar hitters while marking outliers (noise).
3. **Dimensionality Reduction (PCA)** — Reduces high-dimensional swing and power metrics to principal components for visualization and clustering.
4. **Label Propagation on Graphs** — Builds a similarity graph of hitters and uncovers communities using iterative label spreading.

These methods allow us to segment players into meaningful groups and visualize offensive tendencies without needing outcome labels like WAR or All-Star status.
