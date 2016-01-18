# enumerateblood
A multi-response Gaussian model capable of accurately estimating the composition of blood samples from their gene expression profiles. Fit on Affymetrix Gene ST gene expression profiles using the glmnet R package.

Usage:

```
library(devtools)
install_github('cashoes/enumerateblood')

library(enumerateblood)
data('enumerateblood')

predict(model, x)
```
