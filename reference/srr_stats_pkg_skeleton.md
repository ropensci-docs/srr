# Make skeleton package to test roclet system

Make a dummy package skeleton including 'srr' roxygen2 tags which can be
used to try out the functionality of this package. Running the example
lines below which activate the 'srr' roclets, and show you what the
output of those roclets looks like. Feel free to examine the effect of
modifying any of the `@srrstats` tags within the code as identified by
running those lines.

## Usage

``` r
srr_stats_pkg_skeleton(base_dir = tempdir(), pkg_name = "demo")
```

## Arguments

- base_dir:

  The base directory where the package should be constructed.

- pkg_name:

  The name of the package. The final location of this package will be in
  `file.path(base_dir, pkg_name)`.

## Value

The path to the directory holding the newly created package

## See also

Other helper:
[`srr_stats_categories()`](https://docs.ropensci.org/srr/reference/srr_stats_categories.md),
[`srr_stats_checklist()`](https://docs.ropensci.org/srr/reference/srr_stats_checklist.md),
[`srr_stats_checklist_check()`](https://docs.ropensci.org/srr/reference/srr_stats_checklist_check.md),
[`srr_stats_pre_submit()`](https://docs.ropensci.org/srr/reference/srr_stats_pre_submit.md)

## Examples

``` r
d <- srr_stats_pkg_skeleton (pkg_name = "mystatspkg")
# (capture.output of initial compliation messages)
# \donttest{
x <- utils::capture.output (roxygen2::roxygenise (d), type = "output")
#> ℹ Setting Config/roxygen2/version to "8.1.0"
#> Writing NAMESPACE
#> ℹ Loading mystatspkg
#> ℹ Re-compiling mystatspkg (debug build)
#> ──────────────────── rOpenSci Statistical Software Standards ───────────────────
#> 
#> ── @srrstats standards (8 / 12): 
#>   * [G1.1, G1.2, G1.3, G2.0, G2.1] in function 'test_fn()' on line#11 of file [R/test.R]
#>   * [RE2.2] on line#2 of file [tests/testthat/test-a.R]
#>   * [G2.3] on line#8 of file [src/cpptest.cpp]
#>   * [G1.4] on line#17 of file [README.Rmd]
#> 
#> ── @srrstatsNA standards (1 / 12): 
#>   * [RE3.3] on line#5 of file [R/srr-stats-standards.R]
#> 
#> ── @srrstatsTODO standards (3 / 12): 
#>   * [RE4.4] on line#14 of file [R/srr-stats-standards.R]
#>   * [RE1.1] in function 'test_fn()' on line#11 of file [R/test.R]
#>   * [G1.5] on line#17 of file [README.Rmd]
#> ────────────────────────────────────────────────────────────────────────────────
#> Writing mystatspkg-package.Rd
#> Writing test_fn.Rd
#> Writing NAMESPACE
# }
unlink (d, recursive = TRUE)
```
