<center>
<h1>How to train your model faster and better with Batch Gradient Descent</h1>
</center>

Gradient descent is one of the most popular optimization algorithms in machine learning. It is used to find the optimal parameters of a model that minimize a cost function. However, there are different ways to implement gradient descent, and each one has its pros and cons. In this post, we will focus on one of them: batch gradient descent.

Batch gradient descent is a variant of gradient descent that uses the entire training data to update the parameters in each iteration. This can lead to faster and more stable convergence, but it can also be slow and expensive when the data is large. In this post, we will explain what batch gradient descent is, how it works, and what are its advantages and disadvantages. We will also show you how to implement it in Python using NumPy.

## What is Batch Gradient Descent?

Batch gradient descent is a variant of gradient descent that uses the entire training data to update the parameters in each iteration. The idea is to compute the gradient of the cost function with respect to the parameters using all the training examples, and then move the parameters in the opposite direction of the gradient by a small amount. This process is repeated until the cost function converges to a minimum or a satisfactory value.

For example, let’s say we have a linear regression model that predicts the output y given the input x using a parameter vector theta. The cost function for this model is the mean squared error:

$$\large J(\theta) = \frac{1}{m}\sum_{i=1}^{m}(h_{\theta}(x_i) - y_i)^2$$

where $m$ is the number of training examples, $h_{\theta}(x)$ is the prediction function, and $x_i$ and $y_i$ are the i-th input and output respectively.

The gradient of the cost function concerning theta is:

$$\large \delta$$