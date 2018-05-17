# mr.raps

*mr.raps* is an R package for two-sample Mendelian randomization using the robust adjusted profile score. To install the package, run


```
library(devtools)
install_github("qingyuanzhao/mr.raps")
```

The main function is *mr.raps*. You can find examples by running

```
library(mr.raps)
example(mr.raps) ## Recommended procedure
example(mr.raps.shrinkage) ## General function for empirical partially Bayes estimator
```

In May 2018, a new general function *mr.raps.shrinkage* is added. You can choose whether weight shrinkage should be used using the option *shrinkage*. You can still use the original MR-RAPS procedure using the function *mr.raps.v1*, which is basically the same as setting *shrinkage = FALSE* in *mr.raps.shrinkage*.

References:
* Zhao, Qingyuan, Jingshu Wang, Jack Bowden, and Dylan S. Small. "Statistical inference in two-sample summary-data Mendelian randomization using robust adjusted profile score." arXiv preprint arXiv:1801.09652 (2018).
* Zhao, Qingyuan, Yang Chen, Jingshu Wang, and Dylan S. Small. "Powerful genome-wide design and robust statistical inference in two-sample summary-data Mendelian randomization." arXiv preprint arXiv:1804.07371 (2018).