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
1. $X_{t+1}$ = new value of x after updated
2. $X_t$ = current value of x
3. $\alpha$ = learning rate
4. $\nabla$ = gradient with respect to x

There are several types of gradient descent, including:
1. batch gradient descent
2. stochastic gradient descent (SGD)
3. mini-batch gradient descent

# Batch gradient descent
Batch gradient descent is a type of gradient descent that update the parameters after forward and backward pass through the entire dataset. It is called “batch” gradient descent because it uses the entire dataset to compute the gradient of the loss function at each iteration. Batch gradient descent can be formulated as follows:
$$X_{t+1}=X_t - \alpha \sum_{1}^{n}\nabla$$

Where n is the number of samples in the entire dataset.

One of the main disadvantages of batch gradient descent is that it can be computationally expensive when the dataset is very large, as it requires a forward and backward pass through the entire dataset at each iteration.

In addition, if the dataset is noisy or has a lot of outliers, the loss function can oscillate and never converge to a minimum. In this case, a more sophisticated optimization algorithm such as stochastic gradient descent or mini-batch gradient descent may be more appropriate.

# Stochastic gradient descent (SGD)
Unlike batch gradient descent, which uses the entire dataset to compute the gradient of the loss function at each iteration, SGD uses only one training sample at a time to update the parameters of the model.

SGD can be formulated as follows:
$$X_{t+1}=X_t - \alpha \nabla$$

One advantage of SGD over batch gradient descent is that it is computationally more efficient, as it requires only one forward and backward pass through the model for each training sample, rather than the entire dataset. Additionally, SGD can be implemented online, which means it can update the model parameters on-the-fly as new data arrives.

However, one disadvantage of SGD is that the cost function can oscillate and not converge to a minimum due to the high variance in the updates caused by the use of only one sample at a time. This can be mitigated by using a smaller learning rate and by using mini-batch gradient descent, which combines the benefits of both SGD and batch gradient descent.

# Mini-batch gradient descent
Mini-batch gradient descent is a compromise between batch gradient descent and stochastic gradient descent. Unlike batch gradient descent, which uses the entire dataset to compute the gradient of the loss function at each iteration, and SGD, which uses only one sample at a time, mini-batch gradient descent uses a small subset of the dataset, called a mini-batch, to compute the gradient at each iteration.

Mini-batch gradient descent can be formulated as follows:
$$X_{t+1}=X_t - \alpha \sum_{1}^{n}\nabla$$

Where n is the number of mini-batch or also known as batch size. In the case of mini-batch gradient descent, n must be > 1 and < the total number of samples in the entire dataset.

Mini-batch gradient descent can be seen as a trade-off between stochastic gradient descent and batch gradient descent. It has the advantage that it can reduce the noise of the updates, as the mini-batch is a good representation of the training data and it is less variance than stochastic gradient descent. Moreover, it’s more computationally efficient than batch gradient descent because it uses only a subset of the dataset. However, it is more computationally demanding than stochastic gradient descent, as it requires multiple forward and backward passes through the model for each mini-batch.

A commonly used mini-batch size is between 16 and 256. But the ideal mini-batch size depends on the specific problem and the computational resources available.

# Example
Suppose a function of one variable is as follow: $f(x)=(x-1)^2$ with an initial x₀ of 2 and a learning rate of 0.3. We will do 5 iterations of stochastic gradient descent to minimize function $f(x)$.
![Alt text](https://archive.ph/ia2xk/4a0df411d6f0b26a871865a88420758f786201ca.webp)

Step 1: Find the derivative of $f(x)$ which is $f’(x) = 2(x-1)$
Step 2: Compute the gradient of $f’(x_0)$
$$f'(2) = 2(2-1)$$
$$f'(2) = 2$$
Step 3: Update x using the gradient descent formula
$$X_1 = 2 - (0.3-2)$$
$$X_1 = 1.4

![Alt text](https://archive.ph/ia2xk/3901fd17e66ca023b78c2820ffb913618ecf0350.webp)
