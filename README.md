# AlgorithmicStatMech

Tentative program:

## 1) Dynamic programming
  [Problem sheet](1_dynamic_programming.pdf)
  - Exact solution of chain-factorized models (like 1D ising) via a recursive strategy
  - Exact solution of fully-connected ising or potts with uniform couplings and arbitraty external fields
  - Improvement on the point above by exploiting derivatives (-> automatic differentiation)

 ## 2) Automatic Differentiation (AD)

  - Introduction to the concept, a few motivating examples
  - Implementation via Dual Numbers
  - Dual numbers as a good example of Julia's type dispatch system
  - Hints to reverse-mode AD. Example: backpropagation in neural nets
  - Bonus: reverse-mode AD as message-passing on the computation graph

Two options for the third one:

  ## 3a) Tensor Trains (aka Matrix Product States): a tool for function approximation
  - Can one improve on mean-field ansatzes while keeping the computational advantages?
  - Introduction to tensor trains
  - Efficient computations on tensor trains (dynamic programming): partition function, marginals, sampling
  - Universality of the Tensor Train decomposition
  - SVD-based truncations
  - Bonus: learning of Tensor Train distributions

 ## 3b) Belief Propagation
  - Solution of stat. mech. models on trees, building on the strategy on chains (continuation of part 1)
  - BP on loopy graphs
  - Examples: LDPC decoding or SAT or ising or ...
