# Algorithmic tools for Statistical Mechanics

Material for a mini-course held at Physics Faculty, Universidad de La Habana in February 2024.

## 1) Exact solution of statistical mechanical models via Dynamic Programming
  [Problem sheet](1_dynamic_programming.pdf), [Solution](1_dynamic_programming_solution.pdf)
  - Exact solution of chain-factorized models (like 1D ising) via a recursive strategy
  - Exact solution of fully-connected ising or potts with uniform couplings and arbitraty external fields
  - Improvement on the point above by exploiting derivatives (-> automatic differentiation)

 ## 2) Automatic Differentiation (AD)
[Notebook](2_automatic_differentiation.ipynb)
  - Introduction to the concept, a few motivating examples
  - Implementation via Dual Numbers
  - Dual numbers as a good example of Julia's type dispatch system
  - Hints to reverse-mode AD. Example: backpropagation in neural nets
  - Bonus: reverse-mode AD as message-passing on the computation graph
    
Friendly references:
- https://youtu.be/vAp6nUMrKYg?si=ReQ7qgKugXSZ66Al
- https://book.sciml.ai/notes/08-Forward-Mode_Automatic_Differentiation_(AD)_via_High_Dimensional_Algebras/
- https://www.microsoft.com/en-us/research/video/from-automatic-differentiation-to-message-passing/

References:
- [A Hitchhiker's Guide to Automatic Differentiation](https://arxiv.org/abs/1411.0583)
- [Automatic differentiation in machine learning: a survey](https://arxiv.org/abs/1502.05767)
- [A Differentiable Programming System to Bridge Machine Learning and Scientific Computing](https://arxiv.org/abs/1907.07587)


Two options for the third session:

  ## 3a) Tensor Trains (aka Matrix Product States): a tool for function approximation
  - Can one improve on mean-field ansatzes while keeping the computational advantages?
  - Introduction to tensor trains
  - Efficient computations on tensor trains (dynamic programming): partition function, marginals, sampling
  - Universality of the Tensor Train decomposition
  - SVD-based truncations
  - Bonus: learning of Tensor Train distributions

Friendly references:
- https://www.youtube.com/watch?v=903oLALEDPk
- https://tensornetwork.org/
- https://www.youtube.com/watch?v=AmQNaYhhGss&t=1468s

References:
- [The density-matrix renormalization group in the age of matrix product states](https://arxiv.org/abs/1008.3477)

Reading material:
- [Unsupervised Generative Modeling Using Matrix Product States](https://arxiv.org/abs/1709.01662)
- [Supervised Learning with Quantum-Inspired Tensor Networks](https://arxiv.org/abs/1605.05775)
- [Tropical Tensor Network for Ground States of Spin Glasses](https://arxiv.org/abs/2008.06888)
- [Equivalence of restricted Boltzmann machines and tensor network states](https://arxiv.org/abs/1701.04831)

 ## 3b) Belief Propagation
  - Solution of stat. mech. models on trees, building on the strategy on chains (continuation of part 1)
  - BP on loopy graphs
  - Examples: LDPC decoding or SAT or ising or ...

Friendly references:
- https://www.youtube.com/watch?v=1XSGqkZ54qg&list=PL8mMEmoXNBfaBEMiKdQnTvCLOVRniOrPb&index=36

References:
- [Understanding Belief Propagation and its Generalizations](https://www.merl.com/publications/TR2001-22)
- Information, physics, and computation, M Mezard, A Montanari, Oxford University Press
