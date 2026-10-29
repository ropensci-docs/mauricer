# Is a BEAST2 package installed?

Checks if a BEAST2 package is installed.

## Usage

``` r
is_beast2_pkg_installed(
  name,
  beast2_folder = beastier::get_default_beast2_folder(),
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

- has_internet:

  boolean to indicate if the user has access to the internet. By
  default, this value equals the result of
  [`curl::has_internet`](https://jeroen.r-universe.dev/curl/reference/nslookup.html)

## Value

- `TRUE` if the BEAST2 package is installed

- `FALSE` if the BEAST2 package is not installed

- `NULL` if there is no internet connection

## Details

To be able to check this, an internet connection is needed. Without an
internet connection, `NULL` is returned.

## See also

Use
[is_beast2_ns_pkg_installed](https://docs.ropensci.org/mauricer/reference/is_beast2_ns_pkg_installed.md)
to see if the NS package is installed without an internet connection

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
if (FALSE) { # \dontrun{
  is_beast2_pkg_installed("Beasy")
} # }
```
