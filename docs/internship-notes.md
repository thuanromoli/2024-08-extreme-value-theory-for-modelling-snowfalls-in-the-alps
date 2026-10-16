# Prerequisites
- Read "Introduction to extreme value theory"
- Read "[tail index regression](https://www.tandfonline.com/doi/abs/10.1198/jasa.2009.tm08458)" and "[Generalised pareto regression trees](https://link.springer.com/article/10.1007/s10687-024-00485-1)"
- Read "[flood modelling](https://arxiv.org/abs/2208.07590)" and "[Wildfires in Europe](https://journals.ametsoc.org/view/journals/aies/2/4/AIES-D-22-0095.1.xml)"

# Week 1: 22-26 July
- Learn about machine learning methods
- Read papers and code
	- [Generalised pareto regression trees](https://link.springer.com/article/10.1007/s10687-024-00485-1) with [code](https://github.com/antoine-heranval/Generalized-Pareto-Regression-Trees-for-extreme-event-analysis)
	- [Cyber claim analysis using Generalized Pareto regression trees with applications to insurance](https://www.sciencedirect.com/science/article/pii/S0167668721000330) with [code](https://bitbucket.org/sebastien_farkas/cyber_claim_analysis_gpd_regression_trees/src/master/)
- Exploratory analysis on [our data set](https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels-monthly-means?tab=overview)

# Week 2: 29-02 Aug
- Questions:
	- Heterogeneity
	- Loss function $\phi$
	- CART algorithm
	- how would you use trees to do inference, usually we re-parametrise the parameters of a distribution with a vector of parameters associated to each covariate. Then get parameters that minimise the joint likelihood.
- Data set:
		- how to map using ggplot, gridded data
		- how to use dates
		- what are the covariates (dates, lonlat, others)

# Week 3: 5-9 Aug
- Fit GPD intercept only model
- Work with the dataset, transform from 3d spatial, temporal to long format

# Week 4: 12-16 Aug
- Fit GPD model with covariates and continue explanatory analysis
- Start looking at regression trees code

# Week 5: 19-23 Aug
- Try to get regression trees to work
- Do model selection and start explanation of data

# Week 6: 26-30 Aug
- Code k-fold cross-validation with k=5 to do model selection
- Non-parametric bootstrapping of estimates
- Write conclusion on
	- Shape parameter
	- significant coefficients in scale parameters
	- spacial map of scale parameter
