# Logistic Regression

Logistic Regression is a supervised learning algorithm used for binary classification tasks. It estimates the probability that a given input belongs to a particular class. Unlike linear regression, which predicts continuous values, logistic regression predicts discrete binary outcomes (e.g., 0 or 1, True or False).

## Sigmoid Function

The core of logistic regression is the sigmoid function. It maps any real-valued number inot a value between 0 and 1

<p align="center">
$\sigma (z) = \frac{1}{1 + e^{-z}}$
</p>

where $z$ is a linear combination of input features

## Cost Function

Instead of using mean squared error used in linear regression, logistic regression uses the log-loss (also known as binary cross-entropy)  to penalize wrong predictions:

<p align="center">
$J(\theta) = - \frac{1}{m} \sum_{i=1}{m} [ y^{(i)} log(h_{\theta}(x^{(i)})) + (1 - y^{(i)})log(1 - h_{\theta}(x^{(i)}))]$
</p>

## Optimization
The parameter $\theta$ are optimized using Gradient Descent
