---
title: Gradient Descent Simplified
author: Mgs M Luthfi Ramadhan
tags:
  - Data Science
  - Artificial Intelligence
  - Machine Learning
  - NLP
  - Data
---
<!-- excerpt start -->
Gradient descent is an optimization algorithm used to minimize a function. Gradient descent works by iteratively moving in the direction opposite to the gradient of the function, with the step size determined by a hyperparameter called “learning rate”. Gradient descent is commonly used in machine learning to adjust the parameters of a model in order to minimize the loss function, especially in deep learning. In deep learning, gradient descent will adjust every trainable weights and biases of the model in which when these weights and biases are used, the loss function will be minimum.
<!-- excerpt end -->

Mathematically speaking, gradient descent can be formulated as follow:
$$X_{t+1}=X_t - \alpha \nabla$$

where,
$X_{t+1}$ = new value of x after updated
$X_t$ = current value of x
$\alpha$ = learning rate
$\nabla$ = gradient with respect to x

There are several types of gradient descent, including:
1. batch gradient descent
2. stochastic gradient descent (SGD)
3. mini-batch gradient descent

# Batch gradient descent
Batch gradient descent is a type of gradient descent that update the parameters after forward and backward pass through the entire dataset. It is called “batch” gradient descent because it uses the entire dataset to compute the gradient of the loss function at each iteration. Batch gradient descent can be formulated as follows:
$$X_{t+1}=X_t - \alpha \sum_{1}^{n}\nabla$$

