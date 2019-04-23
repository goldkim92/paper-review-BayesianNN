## Sparse Guassian Processes using Pseudo-inputs (SPGP)
[paper]() by Edward Snelson and Zoubin Ghahramani, from University College London

## Abstract
**new approach by introducing pseudo-input points learned by optimization**
> We present a new Gaussian Process (GP) regression model whose covariance is parameterized by the locations of M pseudo-input points, which we learn by gradient based optimization. We take M << N, where N is the number of real data points, and hence optain a sparse regression method which has O(M^2*N) training cost and O(M^2) prediction cost per test case. We also find hyperparameters of the covariance function in the same joint optimization. The method can be viewed as a Bayesian regression model with particular input dependent noise.

**comparison with other sparse GP methods**
> The method turns out to be closely related to several other sparse GP approaches, and we discuss the relation in detail.

**demonstrate the performance with several experiments**
> We finally demonstrate its performance on some large data sets, and make a direct comparison to other sparse GP methods. We show that our method can match full GP performance with small M, i.e. very sparse solutions, it significantly outperforms other approaches in this regime.


## Method
Similar with predictive distribution in GP (figure a) regression model, SPGP (figure b) calculates predictive distribution based on M pseudo-inputs and hyperparemeters composed in the covariance function. M pseudo-inputs and hyperparameters are opitmized in gradient ascent method by maximizing the marginal likelihood. As a result, adversarially chosen initial M pseudo-inputs (red crosses) spread along the extent of the training data (blue crosses)

![](img/img1.png)
