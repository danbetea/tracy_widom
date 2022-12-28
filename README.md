# tracy_widom  

This Mathematica project numerically computes the Tracy--Widom GUE (Gaussian Unitary Ensemble) and GOE (Gaussian Orthogonal Ensemble) cumulative distribution functions using the Fredholm determinant method of Bornemann. 

A brief lay description of the Tracy--Widom distributions appears in [this Quanta Magazine article](https://www.quantamagazine.org/beyond-the-bell-curve-a-new-universal-law-20141015/). The GUE distribution first appeared in the work of Tracy and Widom, *Level-Spacing Distributions and the Airy Kernel*, [arXiv:hep-th/9211141](https://arxiv.org/abs/hep-th/9211141); and in the work of Forrester, *The spectrum edge of random matrix ensembles*, [article available here](https://www.sciencedirect.com/science/article/abs/pii/055032139390126A) (paywalled). The GOE distribution appeared in Tracy and Widom, *On Orthogonal and Symplectic Matrix Ensembles*, [arXiv:solv-int/9509007](https://arxiv.org/abs/solv-int/9509007).

The details of the numerical method can be found in the work of Bornemann, *On the Numerical Evaluation of Fredholm Determinants*, [arXiv:0804.2543v2 math.NA](https://arxiv.org/abs/0804.2543).

The implementation agrees with the built-in Mathematica implementation (based on Painlevé transcendents as far as I know) to 6 digits save for the left tail (where the distribution function is exponentially close to 0). The method needs refinement to handle left tails properly.
