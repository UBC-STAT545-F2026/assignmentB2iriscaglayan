
<!-- README.md is generated from README.Rmd. Please edit that file -->

# assignmentB2iriscaglayan

assignmentB2iriscaglayan counts missing values in every column except
the grouping column, grouped by a specified column. It helps users
summarize and compare missing data across groups. \## Installation

You can install version 0.1.0 of assignmentB2iriscaglayan from

``` r
# Install if needed:
# install.packages("devtools")

devtools::install_github(
  "UBC-STAT545-F2026/assignmentB2iriscaglayan",
  ref = "0.1.0"
)
```

## Example

Count missing values in the airquality dataset grouped by month

``` r
library(assignmentB2iriscaglayan)
## basic example code
count_all_missing_by_group(airquality, Month)
#> # A tibble: 5 × 6
#>   Month Ozone Solar.R  Wind  Temp   Day
#>   <int> <int>   <int> <int> <int> <int>
#> 1     5     5       4     0     0     0
#> 2     6    21       0     0     0     0
#> 3     7     5       0     0     0     0
#> 4     8     5       3     0     0     0
#> 5     9     1       0     0     0     0
```
