# srr_stats_roclet

Get values of all `srrstats` tags in function documentation

## Usage

``` r
srr_stats_roclet()
```

## Value

A roxygen2 roclet

## Details

Note that this function should never need to be called directly. It only
exists to enable "@srrstats" tags to be parsed from roxygen2
documentation.

## See also

Other roxygen:
[`srr_stats_roxygen()`](https://docs.ropensci.org/srr/reference/srr_stats_roxygen.md)

## Examples

``` r
srr_stats_roclet ()
#> list()
#> attr(,"class")
#> [1] "roclet_srr_stats" "roclet"          
```
