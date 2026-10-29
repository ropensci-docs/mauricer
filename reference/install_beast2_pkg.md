# Install a BEAST2 package

Install a BEAST2 package. If the package is already installed, (see
[is_beast2_pkg_installed](https://docs.ropensci.org/mauricer/reference/is_beast2_pkg_installed.md)),
this function [stop](https://rdrr.io/r/base/stop.html)s.

## Usage

``` r
install_beast2_pkg(
  name,
  beast2_folder = beastier::get_default_beast2_folder(),
  verbose = FALSE,
  has_internet = curl::has_internet()
)
```

## Arguments

- name:

  the package's name

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

- verbose:

  set to TRUE for extra output, as can be used in debugging

- has_internet:

  boolean to indicate if the user has access to the internet. By
  default, this value equals the result of
  [`curl::has_internet`](https://jeroen.r-universe.dev/curl/reference/nslookup.html)

## Value

nothing. It does install the BEAST2 package

## Note

Installing or uninstalling a BEAST2 package for a (singular) BEAST2
installation, does so for all BEAST2 installations

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
if (FALSE) { # \dontrun{
  install_beast2_pkg("NS")
} # }
```
