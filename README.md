# tracy_widom  

This project (the Mathematica file `tracy_widom.nb`) numerically computes the Tracy--Widom GUE (Gaussian Unitary Ensemble) and GOE (Gaussian Orthogonal Ensemble) distributions using the Fredholm determinant method of Bornemann. 

A brief lay description of the Tracy--Widom distributions appears in this Quanta Magazine article: https://www.quantamagazine.org/beyond-the-bell-curve-a-new-universal-law-20141015/. The GUE distribution first appeared in this article by Tracy--Widom (*Level-Spacing Distributions and the Airy Kernel*, **arXiv:hep-th/9211141**, available at https://arxiv.org/abs/hep-th/9211141) and this article by Forrester (*The spectrum edge of random matrix ensembles*, https://www.sciencedirect.com/science/article/abs/pii/055032139390126A). The GOE distribution appeared slightly later, still introduced by Tracy--Widom (*On Orthogonal and Symplectic Matrix Ensembles*, **arXiv:solv-int/9509007**, available at https://arxiv.org/abs/solv-int/9509007).

The details of the numerical method can be found in Bornemann, *On the Numerical Evaluation of Fredholm Determinants*, **arXiv:0804.2543v2 [math.NA]**, available at https://arxiv.org/abs/0804.2543.

The implementation is in Mathematica (so far!), and it agrees with the built-in implementation (based on Painlevé transcendents as far as I know) to 6 digits save for the left tail (where the distribution function is exponentially close to 0). The method needs a bit of refinement to handle left tails properly (and/or my Mathematica code is a bit naïve in the computations). 

I hope to be able to translate the code into Python (+sage perhaps), Julia, and/or Matlab at some point. 
