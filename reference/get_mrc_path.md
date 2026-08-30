# Get the full path of a `mauricer` file

Get the full path of a file in the `inst/extdata` folder. If there is no
`mauricer` file, get_mrc_path will
[stop](https://rdrr.io/r/base/stop.html).

## Usage

``` r
get_mrc_path(filename)
```

## Arguments

- filename:

  the file's name, without the path

## Value

the full path of the filename, if and only if the file is present. Will
stop otherwise.

## See also

for more files, use
[`get_mrc_paths`](https://docs.ropensci.org/mauricer/reference/get_mrc_paths.md)

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
get_mrc_path("anthus_aco_sub.fas")
#> [1] "/github/home/R/x86_64-pc-linux-gnu-library/4.6/mauricer/extdata/anthus_aco_sub.fas"
```
