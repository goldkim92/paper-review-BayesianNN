## Gaussian Variational Approximation with a factor covariance structure (VAFC)
[paper](https://arxiv.org/pdf/1701.03208.pdf) by Victor M.-H. Ong, David J.Nott, and Michael S. Smith 
from National University of Singapore

### Abstract
**general description**
> Variational approximation methods have proven to be useful for scaling Bayesian 
computations to large data sets and highly parameterized models. Applying variational 
methods involves solving an optimization problem, and recent research in this area has 
focused on stochastic gradient ascent methods as a general approach to implementation.

**restrict variational approximation to a Gaussian approximation and define the problem**
> Here variational approximation is considered for a posterior distribution in high 
dimensions using a Gaussian approximating family. Gaussian variational approximation 
with an unrestricted covariance matrix can be computationally burdensome in many problems 
because the number of elements in the covariance matrix increases quadratically with 
the dimension of the model parameter. 

**solve it by low-dimensional factor covarianc structures**
> To circumvent this problem, low-dimensional factor covariance structures are considered.
General stochastic gradient approaches to efficiently perform the optimization are described, 
with gradient estimates obtained using so-called "reparameterization trick". 

**results with several experiment**
> The end result is a flexible and efficient approach to high-dimensional Gaussian variational 
approximation, which we illustrate using eight real datasets.

