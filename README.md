# Extreme value theory for modelling snowfalls in the Alps

## Description

This repository contains the project I undertook during my internship at the University of Edinburgh (Summer 2024), under the supervision of Dr Jordan Richards.


## Abstract

Extreme value analysis (EVA) has emerged as one of the most important statistical disciplines for the applied sciences over the last 50 years. The distinguishing feature of EVA is the objective to quantify the stochastic behaviour of a process at unusually large, or small, levels. In particular, EVA usually require estimation of the probability of events that are more extreme than any that have already been observed.

In this project, we produce R code to model extreme snowfalls in the Italian Alps using a specific EVA model called threshold model. We predict an upper bound for the snowfall received in each region, and we investigate which covariates are statistically significant for snowfalls.

## Repository contents

- [Full report](report.pdf) and [LaTeX source with figures](latex.zip).
- [R Markdown notebook](code/code.Rmd), with the snowfall and elevation datasets in `code/`.
- [Internship reading list and weekly research notes](docs/internship-notes.md).
- [Project summary in Word format](docs/project-summary.docx).
- Research material in `docs/`: [handwritten notes](docs/Notes.xopp), [introduction to EVA](docs/intro%20to%20EVA.pdf), [Generalized Pareto regression trees](docs/GP%20reg%20trees%20for%20EVA.pdf), [cyber claim analysis](docs/Cyber%20claim%20analysis%20using%20Generalized%20Pareto%20regression%20trees%20with%20applications%20to%20insurance.pdf), and [ismev documentation](docs/ismev.pdf).

## Running the notebook

Use R with the following packages installed:

```r
install.packages(c("ggplot2", "ggmap", "texmex", "ismev", "rmarkdown", "knitr"))
```

To work interactively, open `code/code.Rmd` and set the R working directory to `code/`. The notebook loads `Alps_precip.Rdata` and `elev.Rdata` using relative paths.

To render an HTML copy, run these commands from the repository root with Pandoc available (for example, through RStudio):

```sh
cd code
Rscript -e 'rmarkdown::render("code.Rmd")'
```

The notebook includes repeated model fitting, bootstrapping, and cross-validation, so a full render may take some time. No pre-rendered notebook is included.

## Project consolidation

The internship notes, project summary, and research material were consolidated from `2024-08-edinburgh-university`. The R Markdown notebook and both datasets were identical in the two repositories. This repository retains its existing report and LaTeX source, including the title punctuation update. The old rendered HTML and local R session histories were excluded.
