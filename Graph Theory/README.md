# Graph Theory

This section applies two key graph algorithms to MLB Statcast data to uncover structure in player similarity:

1. **Label Propagation** – identifies clusters of similar players.
2. **Maximum Clique Detection** – finds the most tightly connected group of players.


## Label Propagation

Label Propagation is an iterative algorithm for unsupervised community detection. Each node adopts the label most common among its neighbors until convergence.

- **Time Complexity:** \( \mathcal{O}(|E|) \)
- **Strengths:** Fast, scalable, and effective for discovering naturally forming player groups


## Maximum Clique (via MILP)

A **clique** is a set of nodes all directly connected to each other. The **maximum clique** is the largest such set.

- **Formulation:** MILP with binary variables and pairwise constraints
- **Solves:**  
  \[
  \max \sum x_i \quad \text{subject to} \quad x_i + x_j \leq 1 \; \text{if } (i, j) \notin E
  \]
