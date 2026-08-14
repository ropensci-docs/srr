# Perform pre-submission checks

Check that all standards are present in code, and listed either as
'@srrstats' or '@srrstatsNA'

## Usage

``` r
srr_stats_pre_submit(path = ".", quiet = FALSE)
```

## Arguments

- path:

  Path to local repository to check

- quiet:

  If 'FALSE', display information on status of package on screen.

## Value

(Invisibly) List of any standards missing from code

## See also

Other helper:
[`srr_stats_categories()`](https://docs.ropensci.org/srr/reference/srr_stats_categories.md),
[`srr_stats_checklist()`](https://docs.ropensci.org/srr/reference/srr_stats_checklist.md),
[`srr_stats_checklist_check()`](https://docs.ropensci.org/srr/reference/srr_stats_checklist_check.md),
[`srr_stats_pkg_skeleton()`](https://docs.ropensci.org/srr/reference/srr_stats_pkg_skeleton.md)

## Examples

``` r
d <- srr_stats_pkg_skeleton ()
# The skeleton has 'TODO' standards, and also has only a few from the full
# list expected for the categories specified there.
# \donttest{
srr_stats_pre_submit (d)
#> ✖ This package still has TODO standards and can not be submitted
#> ! Package can not be submitted because the following standards [v0.2.0] are missing from your code:
#> 1. G1.0
#> 2. G1.4a
#> 3. G1.6
#> 4. G2.0a
#> 5. G2.1a
#> 6. G2.2
#> 7. G2.3a
#> 8. G2.3b
#> 9. G2.4
#> 10. G2.4a
#> 11. G2.4b
#> 12. G2.4c
#> 13. G2.4d
#> 14. G2.4e
#> 15. G2.5
#> 16. G2.6
#> 17. G2.7
#> 18. G2.8
#> 19. G2.9
#> 20. G2.10
#> 21. G2.11
#> 22. G2.12
#> 23. G2.13
#> 24. G2.14
#> 25. G2.14a
#> 26. G2.14b
#> 27. G2.14c
#> 28. G2.15
#> 29. G2.16
#> 30. G3.0
#> 31. G3.1
#> 32. G3.1a
#> 33. G4.0
#> 34. G5.0
#> 35. G5.1
#> 36. G5.2
#> 37. G5.2a
#> 38. G5.2b
#> 39. G5.3
#> 40. G5.4
#> 41. G5.4a
#> 42. G5.4b
#> 43. G5.4c
#> 44. G5.5
#> 45. G5.6
#> 46. G5.6a
#> 47. G5.6b
#> 48. G5.7
#> 49. G5.8
#> 50. G5.8a
#> 51. G5.8b
#> 52. G5.8c
#> 53. G5.8d
#> 54. G5.9
#> 55. G5.9a
#> 56. G5.9b
#> 57. G5.10
#> 58. G5.11
#> 59. G5.11a
#> 60. G5.12
#> 61. RE1.0
#> 62. RE1.2
#> 63. RE1.3
#> 64. RE1.3a
#> 65. RE1.4
#> 66. RE2.0
#> 67. RE2.1
#> 68. RE2.3
#> 69. RE2.4
#> 70. RE2.4a
#> 71. RE2.4b
#> 72. RE3.0
#> 73. RE3.1
#> 74. RE3.2
#> 75. RE4.0
#> 76. RE4.1
#> 77. RE4.2
#> 78. RE4.3
#> 79. RE4.5
#> 80. RE4.6
#> 81. RE4.7
#> 82. RE4.8
#> 83. RE4.9
#> 84. RE4.10
#> 85. RE4.11
#> 86. RE4.12
#> 87. RE4.13
#> 88. RE4.14
#> 89. RE4.15
#> 90. RE4.16
#> 91. RE4.17
#> 92. RE4.18
#> 93. RE5.0
#> 94. RE6.0
#> 95. RE6.1
#> 96. RE6.2
#> 97. RE6.3
#> 98. RE7.0
#> 99. RE7.0a
#> 100. RE7.1
#> 101. RE7.1a
#> 102. RE7.2
#> 103. RE7.3
#> 104. RE7.4
#> ! Standards should be documented in most package files, yet are mostly only documented in one file.
#> ! Package must comply with at least 50% of all standards, but currently complies with only 7%
#> ! Package must comply with at least 50% of category-specific standards, but currently complies with only 7%
# }
unlink (d, recursive = TRUE)
```
