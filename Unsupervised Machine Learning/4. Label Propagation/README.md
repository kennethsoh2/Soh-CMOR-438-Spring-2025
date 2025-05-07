# Label Propagation

**Label Propagation** is a graph-based semi-supervised learning algorithm that detects communities by spreading labels through a network. Initially, each node is assigned a unique label. Then, in each iteration, every node adopts the most common label among its neighbors. This process repeats until convergence.

The method is efficient and scalable, relying solely on the structure of the graph — it does not require labeled training data or a specific number of communities in advance.

In this project, we construct a **similarity graph of MLB hitters** based on their swing characteristics, specifically Swing% and O-Swing%. Players are connected if their profiles are sufficiently similar (within a given distance threshold), and label propagation is used to identify natural clusters or player communities within this graph.

This approach is particularly useful for understanding groups of hitters with similar swing approaches, even without explicit labeling of roles or outcomes.
