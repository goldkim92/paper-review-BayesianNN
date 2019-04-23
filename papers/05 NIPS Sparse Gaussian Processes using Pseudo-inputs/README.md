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
The predictive distribution of GP regression is
<a href="https://www.codecogs.com/eqnedit.php?latex=p(y|x,D)=N(y|k_x^T(K_N&plus;\sigma^2I)^{-1}&space;y,&space;K_{xx}-k_x^T(K_N&plus;\sigma^2I)^{-1}k_x&plus;\sigma^2)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?p(y|x,D)=N(y|k_x^T(K_N&plus;\sigma^2I)^{-1}&space;y,&space;K_{xx}-k_x^T(K_N&plus;\sigma^2I)^{-1}k_x&plus;\sigma^2)" title="p(y|x,D)=N(y|k_x^T(K_N+\sigma^2I)^{-1} y, K_{xx}-k_x^T(K_N+\sigma^2I)^{-1}k_x+\sigma^2)" /></a>
