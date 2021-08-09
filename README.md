# tracy_widom
This project computes the Tracy--Widom  GUE and GOE distributions using the Fredholm determinant method of Bornemann.

The details can be found in F. Bornemann, 'On the Numerical Evaluation of Fredholm Determinants', **arXiv:0804.2543v2 [math.NA]**, available at https://arxiv.org/abs/0804.2543 

The implementation is in Mathematica (so far!), and it agrees with the built in implementation (based on Painlevé transcendents) to 6 digits save for the left tail (where the distribution function is exponentially close to 0). The method needs a bit of refinement to handle left tails properly (and/or my Mathematica code is a bit naïve in the computations). 

I hope to be able to translate the code into Python (+sage perhaps), Julia, and/or Matlab at some point. 
