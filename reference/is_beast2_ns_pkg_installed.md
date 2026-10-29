# Is the BEAST2 NS package installed?

Determine if the BEAST2 NS package is installed.

## Usage

``` r
is_beast2_ns_pkg_installed(
  show_warnings = FALSE,
  verbose = FALSE,
  beast2_folder = beastier::get_default_beast2_folder()
)
```

## Arguments

- show_warnings:

  set to TRUE to show warnings

- verbose:

  set to TRUE for extra output, as can be used in debugging

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

## Value

TRUE if the BEAST2 NS package is installed, FALSE otherwise

## Details

Unlike
[is_beast2_pkg_installed](https://docs.ropensci.org/mauricer/reference/is_beast2_pkg_installed.md),
this function does not need an internet connection. Instead, the
function calls BEAST2 to read a BEAST2 XML file that uses NS.

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
if (FALSE) { # \dontrun{
  is_beast2_ns_pkg_installed()
} # }
```
