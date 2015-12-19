# bnps

This repository houses the `R` package `bnps`, which is used for fitting Bayesian nonparametric adaptive smoothing models as described in Faulkner and Minin (2015).  The `bnps` package interfaces with Stan, which is a C++ package for performing Bayesian inference using Hamiltonian Monte Carlo (see [http://mc-stan.org/](http://mc-stan.org/)).  Stan can be interfaced with the R package `rstan`, and thus the `bnps` package depends on the `rstan` package to fit models.

## Installation
1. Install package dependency `rstan` and install package `devtools` using `install.packages` function.  Note that if you do not already have `rstan` installed, you may need to install additional packages such as `Rtools` if using a Windows platform, or `Xcode` if you are using a Mac.  See the [`rstan` prerequisites](https://github.com/stan-dev/rstan/wiki/RStan-Getting-Started#prerequisites) for more information.  If you want the vignettes, you may also need to install the 'rmarkdown' package
2. Load `devtools` using `library(devtools)`.
3. Install `bnps` from GitHub using either
  1. `install_github("jrfaulkner/bnps")` or
  2. `install_github("jrfaulkner/bnps", build_vignettes=TRUE)` if you want the vignette documentation which provides examples of using `bnps`.  Note that building vignettes will make the load take a little longer.

## Vignettes
The following vignettes provide some examples using the `bnps` package with step-by-step instructions and R code. 

1. **Introduction_to_bnps**
2. **coal_mine_example**
3. **tokyo_rain_example**

## References
Faulkner, J. R., and V. N. Minin. 2015. Bayesian trend filtering: adaptive temporal smoothing with shrinkage priors. arXiv preprint.
