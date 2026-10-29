# Get all BEAST2 package names

List all BEAST2 packages that are available and installed. Will
[stop](https://rdrr.io/r/base/stop.html) if there is no internet
connection

## Usage

``` r
get_beast2_pkg_names(
  beast2_folder = beastier::get_default_beast2_folder(),
  has_internet = curl::has_internet(),
  verbose = FALSE
)
```

## Arguments

- beast2_folder:

  the folder where the BEAST2 is installed. Note that this is not the
  folder where the BEAST2 executable is installed: the BEAST2 executable
  is in a subfolder. Use
  [get_default_beast2_folder](https://docs.ropensci.org/beastier/reference/get_default_beast2_folder.html)
  to get the default BEAST2 folder. Use
  [get_default_beast2_bin_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_bin_path.html)
  to get the full path to the default BEAST2 executable. Use
  [get_default_beast2_jar_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_jar_path.html)
  to get the full path to the default BEAST2 jar file.

- has_internet:

  boolean to indicate if the user has access to the internet. By
  default, this value equals the result of
  [`curl::has_internet`](https://jeroen.r-universe.dev/curl/reference/nslookup.html)

- verbose:

  set to TRUE for extra output, as can be used in debugging

## Value

a data frame with columns

1.  name package name, for example, `bdmm`

2.  installed_version the installed version, for example, `2.6.2`.
    `installed_version` will be NA if the package is not installed

3.  latest_version version number of the latest version, for example,
    `2.6.3`

4.  dependencies packages the package depends on, for example
    `BEASTLabs, GEO_SPHERE`. `dependencies` will be empty if there are
    no dependencies

5.  description description of the package, for example
    `Nested sampling for model selection and posterior inference`

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
if (beastier::is_beast2_installed() && curl::has_internet()) {
  get_beast2_pkg_names()
}
```
