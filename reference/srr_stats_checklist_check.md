# Check a completed standards checklist

Correct any potential formatting issues in a completed standards
checklist

## Usage

``` r
srr_stats_checklist_check(file)
```

## Arguments

- file:

  Name of local file containing a completed checklist. Must be a
  markdown document in `.md` format, not `.Rmd` or anything else.

## Value

(Invisibly) A character vector of markdown-formatted lines containing
the entire checklist of the specified file.

## See also

Other helper:
[`srr_stats_categories()`](https://docs.ropensci.org/srr/reference/srr_stats_categories.md),
[`srr_stats_checklist()`](https://docs.ropensci.org/srr/reference/srr_stats_checklist.md),
[`srr_stats_pkg_skeleton()`](https://docs.ropensci.org/srr/reference/srr_stats_pkg_skeleton.md),
[`srr_stats_pre_submit()`](https://docs.ropensci.org/srr/reference/srr_stats_pre_submit.md)

## Examples

``` r
f <- tempfile (fileext = ".md")
if (FALSE) { # \dontrun{
srr_stats_checklist (category = "regression", filename = f)
chk <- srr_stats_checklist_check (f)
} # }
```
