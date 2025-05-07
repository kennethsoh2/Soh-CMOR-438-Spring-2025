# Ensemble Methods

**Ensemble Methods** combine the outputs of multiple models to improve predictive performance. In this project, we implement a **Gradient Boosting Regressor**, which builds a sequence of shallow decision trees, where each new tree corrects the errors of the previous ensemble.

Each tree is trained on the **residuals** of the current ensemble, and the final prediction is the sum of the outputs of all trees, scaled by a learning rate:

$$
\hat{y} = \sum_{m=1}^{M} \eta \cdot h_m(\mathbf{x})
$$

where $h_m$ is the prediction from the $m$-th tree and $\eta$ is the learning rate.

Boosting is highly effective at reducing both bias and variance, making it a strong choice for **nonlinear regression problems**. However, it is sensitive to overfitting if the number of estimators is too large or the learning rate is too high.

In this project, we use a Boosting Regressor to **predict an MLB player's WAR**, using Statcast-style features like barrel percentage, exit velocity, launch angle, wOBA, and hard hit rate.
