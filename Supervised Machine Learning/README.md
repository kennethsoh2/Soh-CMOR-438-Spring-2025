# Supervised Learning Algorithms

**Supervised Machine Learning** is a class of algorithms that learn from labeled data. In our case, each MLB player in the dataset is associated with a known outcome — such as WAR or All-Star status — which allows us to train models to predict these outcomes based on performance features.

Supervised learning can be split into two main types:
- **Regression**, where the target variable is continuous (e.g., predicting WAR)
- **Classification**, where the target variable is categorical (e.g., classifying a player as an All-Star or not)

In this section, we apply the following supervised learning algorithms to MLB player data:

1. **Perceptron** — Predicts if a player is an All-Star based on Statcast metrics.
2. **Linear Regression** — Predicts a player’s WAR using continuous offensive features.
3. **Logistic Regression** — Classifies players as having over or under 1 WAR.
4. **Neural Networks** — Classifies players as having over or under 2.5 WAR using a feedforward architecture.
5. **K-Nearest Neighbors** — Predicts a player's wRC+ using nearby examples in feature space.
6. **Decision Trees** — Predicts WAR through recursive splits on offensive features.
7. **Random Forests** — Aggregates multiple decision trees to improve WAR prediction accuracy.
8. **Ensemble Methods (Boosting)** — Uses gradient boosting to sequentially improve WAR prediction.

These models demonstrate the power of supervised learning in both interpreting player performance and forecasting future success.
