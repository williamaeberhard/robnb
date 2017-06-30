robNB: an R package for robust estimation and accurate inference for the negative binomial model
------------------------------------------------------------------------------------------------

This R package provides functions for fitting negative binomial generalized linear models to count data both by maximum likelihood and by robust (bounded influence) methods. It also provides many different tests, including saddlepoint tests known for their high accuracy in small samples. For an overview and more details, see the package main help page by running help(robNB) after installation.

Package updates can be found at https://github.com/williamaeberhard/robnb.

Any requests/comments/bug reports should be sent to william.aeberhard@gmail.com.

### Contents

Files contained in this repository:

* robNB_0.2.tar.gz, a tarball containing the R package to be installed from R, see below;
* a LICENSE file;
* this README file.

### Version History

This is robNB version 0.2. The following changes were made from the previous version:

* corrected an error in the computation of st.rob.
* added a stop() statement in st.ml in case the constrained ML fit assigned any fitted.values to maxmu (happens only with really weird samples, made R crash on some systems).

Tested and compiled on R version 3.3.1. R CMD check returned all ok.

### Package Installation

1. Open R.
2. Make sure your working directory contains the file robNB_0.2.tar.gz.
3. Run install.packages('robNB_0.2.tar.gz',repos=NULL,type='source').
4. Load the package by running library(robNB).
5. Check out the main help page by running help(robNB).

### References

Aeberhard, W. H., Cantoni, E. and Heritier, S. (2017) Saddlepoint tests for accurate and robust inference on overdispersed count data. Computational Statistics & Data Analysis (107), 162--175.
