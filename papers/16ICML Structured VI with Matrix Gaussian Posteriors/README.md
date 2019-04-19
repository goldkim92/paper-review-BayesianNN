## Structured and Efficient Variational Deep Learning with Matrix Gaussian Posteriors
[paper](https://arxiv.org/abs/1603.04733) by Christos Louizos and Max Welling, from University of Amsterdam

### Abstract
**The paper is about VBNN with matrix variate Gassian posterior distribution**
> We introduce a variational Bayesian neural netowrk where the parameters are governed via a probability distribution on random matrices. Specifically, we employ a matrix variate Gaussian parameter posterior distribution where we explicitly model the covariance among the input and output dimensions of each layer. 

**This method diminish the learning parameter compared to fully factorized posterior**
> Furthermore, with approximate covariance matrices we can achieve a more efficient way to represent their correlations that is also cheaper than fully factorized parameter posteriors. 

**Interprete the method as Gaussian Process**
> We further show that with the "local reparameterization trick" on this posterior distribution we arrive at a Gaussian Process interpretation of the hidden units in each layer and we, similar with (Gal & Ghahramani, 2015), provide connections with deep Gaussian processes. 

**Efficient posterior sampling by using pseudo-data**
> We continue in taking advantage of this duality and incorporate "pseudo-data" in our model, which in turn allows for more efficient posterior sampling while maintaining the properties of the original model. 

**Several experiments** 
> The valid of the proposed approach is verified through extensive experiments.

