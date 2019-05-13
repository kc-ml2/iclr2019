# Summary of ICLR 2019 by ML2 members

## Mon, May 06
### Representation Learning on Graphs and Manifolds
* https://rlgm.github.io/
* More robust benchmark needed.
* Geometric DL for moleular surfaces
* Many people are using GraphSAGE.
* DGL vs. PyTorch Geometry
* Le Song
  * probabilistic logic over knowledge graph
  * counter-example of GNN not being able to represent MLN exists, but can augment the GNN (for example variational GNN by Le Song) to do the job.
  * UW-CSE dataset
* Leskovec
  * Why graph hard?
    * large
    * non-unique representations of the same graph
    * long-range depedenecies
  * Graph generation baselines
    * Kronecker, MMSB, B-A

## Tue, May 07
* Learning Mixed-Curvature Representations in Product Spaces
  * https://openreview.net/forum?id=HJxeWnCcF7
  * ![poster_20190507_125520](photos/20190507_125520.jpg)
* PyTorch Expo
  * ![slide_2019-05-07_13.30.36](photos/2019-05-07%2013.30.36.jpg)
  * PyTorch BigGraph
    * ![slide_2019-05-07_13.42.17](photos/2019-05-07%2013.42.17.jpg)
  * BoTorch
    * Highly specialized for Bayesian optimization.
    * Not for Bayesian inference therefore no altervative for TFP or Pyro.
    * 1st class support for GPyTorch models.

## Wed, May 08
* Deterministic Variational Inference for Robust Bayesian Neural Networks
  * deterministic VI + empirical ELBO
    * What is empirical ELBO?
* FFJORD
  * uses neural ODE
  * continuous instead of discrete
  * can evolve a unimodal Gaussian into a multimodal complex distribution.
    * But not by a convolution with a static kernel, instead uses time evolution.
  * https://github.com/rtqichen/ffjord
### RL

## Thu, May 09
* seq2tree
  * In fact, AST is also a tree from a sequence of programming language.
  * Linguists don't like sequences, but like trees.
* Embedding representation
  * point
    * no hierarchy
  * Gaussian representation
    * not closed under intersection
  * Cone representation
    * not disjoint
  * Box representation
    * Smoothing the Geometry of Probabilistic Box Embeddings
    * https://openreview.net/forum?id=H1xSNiRcF7
    * how to relate this to the ball representation on the boundary of a hyperbolic space?
* Ordered Neurons: Integrating Tree Structures into Recurrent Neural Networks
  * https://openreview.net/forum?id=B1l6qiR5F7
  * representing a branch of a tree as a stack of nodes
  * cumax
* Poincare GloVe
  * ![poster_2019-05-09_11.23.06](photos/2019-05-09%2011.23.06.jpg)
  * https://openreview.net/forum?id=Ske5r3AqK7
  * relation between Gauissian embedding and half-plane model hyperbolic embedding
    * mapping fixed by an isometry
    * x <-> \mu, y <-> \Sigma
    * semantic meaning by parallel transport, analogous to Euclidean vector arithmetic in a Euclidean word embedding.
