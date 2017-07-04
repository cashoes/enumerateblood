# enumerateblood
A multi-response Gaussian model capable of accurately estimating the composition of blood samples from their gene expression profiles. Fit on Affymetrix Gene ST gene expression profiles using the glmnet R package.

Usage:

```
# install `devtools` if needed with `install.packages('devtools')`
library(devtools)
install_github('cashoes/enumerateblood')

# load package
library(enumerateblood)

# load package data object (the trained model)
data('enumerateblood')

# use the trained model to predict cell proportions
# from gene expression matrix x.
#
# x is a p (probesets) * n (samples) matrix of (RMA) normalized 
# gene expression data (assayed on the Affymetrix Gene 1.0 or 
# 1.1 ST platform), such as that returned by the `oligo::rma()` 
# function
predict(enumerateblood, x)
```
