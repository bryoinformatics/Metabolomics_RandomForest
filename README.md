# Metabolomics_RandomForest (v1.0.0)

Supervised machine learning classification of metabolomic data from poplar using R.

## Contents
- [Summary](#summary)
- [Dependencies](#dependencies)
- [License](#license)
- [Citations](#citations)

Summary
-----
This document contains an example of how one might use a supervised machine learning technique for a classification task. We'll use some targeted metabolomic data collected from *Populus trichocarpa* plants and the random forest algorithm to train a classifier. We can then use this model to classify novel samples based on their metabolite profile and identify which metabolites contribute the most to successful classification.
  
The data were collected from plants grown in a common garden. Samples were collected from the leaves, roots, and rhizosphere (i.e., the soil around the roots). A total of 172 metabolites were measured and each value represents the quantile-normalized metabolite abundance in units of log<sub>10</sub>(LC/MS chromatogram peak height).
  
Random forest is an algorithm that builds many decision trees and combines their output. Bootstrap aggregation (or "bagging") is used to train the model. The "random" part of the algorithm refers to the sampling with replacement of observations and selection of features/predictors used to generate training datasets. This method is great for metabolomics data because it handles high-dimensional datasets efficiently, deals with missing data effectively, is robust to outliers, and doesn't assume the data follow any particular distribution.
  
Our goals here are to (1) develop a model for classifying samples as leaves, roots, or rhizosphere and (2) identify which metabolites are the most important features for classification.

Dependencies
-----
The R notebook (RandomForest.Rmd) is designed to run using the R statistical programming language. 

You can download and install on your computer by following [**this link**](https://mirrors.nics.utk.edu/cran/) (tested on v4.2.1)

You may find it helpful to work within the [**RStudio**](https://posit.co/download/rstudio-desktop/) integrated development environment.

The software packages that are used in this analysis will be automatically downloaded and installed upon execution.

License
-------
This workflow is released under a GNU General Public License (v3.0).

Citations
---------
* Kuhn M (2022). caret: Classification and Regression Training.   R package version 6.0-93, <https://CRAN.R-project.org/package=caret>.
* Liaw A and Wiener M. (2002). Classification and Regression by randomForest. R News 2(3), 18-22.
* R Core Team (2022). R: A language and environment for statistical computing. R Foundation for Statistical Computing, Vienna, Austria. URL https://www.R-project.org/.
* Wickham H. ggplot2: Elegant Graphics for Data Analysis. Springer-Verlag New York, 2016.

