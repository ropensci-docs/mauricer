# Get the full path of one or more `mauricer` files

Get the full paths of files in the `inst/extdata` folder If there is a
`mauricer` file absent, get_mrc_paths will
[stop](https://rdrr.io/r/base/stop.html).

## Usage

``` r
get_mrc_paths(filenames)
```

## Arguments

- filenames:

  the files' names, without the path

## Value

the filenames' full paths

## See also

for one file, use
[`get_mrc_path`](https://docs.ropensci.org/mauricer/reference/get_mrc_path.md)

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
get_mrc_paths(c("anthus_aco_sub.fas", "anthus_nd2_sub.fas"))
#> [1] "/github/home/R/x86_64-pc-linux-gnu-library/4.6/mauricer/extdata/anthus_aco_sub.fas"
#> [2] "/github/home/R/x86_64-pc-linux-gnu-library/4.6/mauricer/extdata/anthus_nd2_sub.fas"
```
