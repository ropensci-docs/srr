# Get details of current statistical software categories

List all currently available categories and associated URLs to full
category descriptions.

## Usage

``` r
srr_stats_categories()
```

## Value

A `data.frame` with 3 columns of "category" (the categories to be
submitted to
[srr_stats_checklist](https://docs.ropensci.org/srr/reference/srr_stats_checklist.md)),
"title" (the full title), and "url".

## See also

Other helper:
[`srr_stats_checklist()`](https://docs.ropensci.org/srr/reference/srr_stats_checklist.md),
[`srr_stats_checklist_check()`](https://docs.ropensci.org/srr/reference/srr_stats_checklist_check.md),
[`srr_stats_pkg_skeleton()`](https://docs.ropensci.org/srr/reference/srr_stats_pkg_skeleton.md),
[`srr_stats_pre_submit()`](https://docs.ropensci.org/srr/reference/srr_stats_pre_submit.md)

## Examples

``` r
srr_stats_categories ()
#>        category std_prefix
#> 1       general          G
#> 2      bayesian         BS
#> 3           eda         EA
#> 4            ml         ML
#> 5    regression         RE
#> 6       spatial         SP
#> 7   time-series         TS
#> 8  unsupervised         UL
#> 9 distributions         PD
#>                                                             title
#> 1                                                         General
#> 2                                                        Bayesian
#> 3                                                             EDA
#> 4                                                Machine Learning
#> 5                              Regression and Supervised Learning
#> 6                                                         Spatial
#> 7                                                     Time Series
#> 8 Dimensionality Reduction, Clustering, and Unsupervised Learning
#> 9                                       Probability Distributions
#>                                                                                                                url
#> 1                                             https://stats-devguide.ropensci.org/standards.html#general-standards
#> 2                             https://stats-devguide.ropensci.org/standards.html#bayesian-and-monte-carlo-software
#> 3                                     https://stats-devguide.ropensci.org/standards.html#exploratory-data-analysis
#> 4                                     https://stats-devguide.ropensci.org/standards.html#machine-learning-software
#> 5                            https://stats-devguide.ropensci.org/standards.html#regression-and-supervised-learning
#> 6                                              https://stats-devguide.ropensci.org/standards.html#spatial-software
#> 7                                          https://stats-devguide.ropensci.org/standards.html#time-series-software
#> 8 https://stats-devguide.ropensci.org/standards.html#dimensionality-reduction-clustering-and-unsupervised-learning
#> 9                                       https://stats-devguide.ropensci.org/standards.html#standards-distributions
```
