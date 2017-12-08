# ENMeval
R package for automated runs and evaluations of ecological niche models.

[`ENMeval`](https://cran.r-project.org/package=ENMeval) is an R package that performs automated runs and evaluations of ecological niche models, and currently implements [Maxent](https://www.cs.princeton.edu/~schapire/maxent/). `ENMeval` was made for those who want to "tune" their models to maximize predictive ability and avoid overfitting, or in other words, optimize model complexity to balance goodness-of-fit and predictive ability. The primary function, `ENMevaluate`, does all the heavy lifting and returns several items including a table of evaluation statistics and, for each setting combination (here, colloquially: *runs*), a model object and a raster layer showing the model prediction across the study extent. There are also options for calculating niche overlap between predictions, running in parallel to speed up computation, and more. For a more detailed description of the package, check out the open-access publication:

[Muscarella, R., Galante, P. J., Soley-Guardia, M., Boria, R. A., Kass, J. M., Uriarte, M. and Anderson, R. P. (2014), ENMeval: An R package for conducting spatially independent evaluations and estimating optimal model complexity for Maxent ecological niche models. Methods in Ecology and Evolution, 5: 1198–1205.](http://onlinelibrary.wiley.com/doi/10.1111/2041-210X.12261/full)

News
===
ENMeval 0.3.0
---
- Changed the default behavior to use the 'maxnet' function of the 'maxnet' package instead of the 'maxent.jar' program.
- Added an algorithm slot to the ENMevaluation object
- Added information on the aggregation factor(s) or number of k folds to the ENMevaluation object when relevant.

