# Deep Neural Network for Classification
Summary of the Deep learning code in Andrew Ng's course  w<sub>1<sub>

This is a classification example by using of deep neural network. In the previous example we made a simple model by Logistic Regression as a Neural Network with 70 percent accuracy. Know we want to improve the model. This is a classification problem with a result of cat and non-cat images.

Two possible models

- 2-layer neural network
- L-Layer deep neural network

At the first part, we will write a code which is composed of 2 hidden layers. At the first layer we have used the RELU activation function and at the seccond layer we used the Sigmoid to produce the classification results. Then we expand this code to L number of hidden layers. We want to see does accucy increases by increasing of the number of layers or not?


# Effect of initialization on the convergence of a Deep Network
For a case of a large number of Weights, it is natural that Z would be really lagre.

z=W<sub>1</sub>X<sub>1</sub> + W<sub>2</sub>X<sub>2</sub>+ W<sub>3</sub>X<sub>3</sub>+..+W<sub>n</sub>X<sub>n</sub>


To  keep z value small we need to use smaller W. Therefore, it is better when the variance of W is eqoual to 1/n .
The solution would be that when we initialize the W with a random numbers, we multiplyit with specific factors.


In this excersize we want to investigate the effect of initialization methodes to the final results of Neural Networks.  Optimized initialization can speed up the gradient descent optimization process and reduce the error. 


# Regularization Techniques
One of the most common problem data science professionals face is to avoid overfitting. Regularization is a technique which makes slight modifications to the learning algorithm such that the model generalizes better. This in turn improves the model’s performance on the unseen data as well.

L2 & L1 regularization
L1 and L2 are the most common types of regularization. These update the general cost function by adding another term known as the regularization term.

Cost function = Loss (say, binary cross entropy) + Regularization term

Due to the addition of this regularization term, the values of weight matrices decrease because it assumes that a neural network with smaller weight matrices leads to simpler models. Therefore, it will also reduce overfitting to quite an extent.

However, this regularization term differs in L1 and L2.
