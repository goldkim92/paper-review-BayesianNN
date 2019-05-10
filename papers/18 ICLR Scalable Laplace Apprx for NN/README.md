## A Scalable Laplace Approximation for Neural Networks
[paper](https://openreview.net/pdf?id=Skdvd2xAZ) by Hippolyt Ritter, Aleksandar Botev, and David Barber, from University College London

## Abstract
**Kronecker factored approximation for the posterior over the weights**
> We leverage recent insights from second-order optimisation for neural networks to construct a Kronecker factored approximation for the posterior over the weights of a trained network. 

**Advantageous for estimating uncertainty without training a new network**
> Our approximation requires no approximation of the training procedure, enabling practitioners to estimate the uncertainty of thier models currently used in practice without having to retrain them. 

**Extensive experiments conducted and provide the efficiency of the proposed method**
> We extensively compare our method to using Dropout and a diagonal Laplace approximation for estimating the uncertainty of a network. We demonstrate that our Kronecker factored method leads to better uncertainty estimates on out-of-distribution data and is more robust to simple adversarial attacks. Our approach only requires calculating two square curvature factor matrices for each layer. Their size is equal to the respective square of the input and output size of the layer, making the method efficient both computationally and in terms of memory usage. We illustrate its scalability by applying it to a state-of-the-art convolutional neural network architecture.  

## Discussion
- Previous work by Louizos and Welling ([summary](papers/16ICML%20Structured%20VI%20with%20Matrix%20Gaussian%20Posteriors)) have also provided new method of BNN using matrix normal distribution. It is interesting to use matrix normal distribution in trained network for estimating the uncertainty. 
- No need to make and train a neural network to assess the uncertainty seems like a huge benefit.
- open review ([link](https://openreview.net/forum?id=Skdvd2xAZ))
