# This function does nothing. It is intended to inherit is parameters' documentation.

This function does nothing. It is intended to inherit is parameters'
documentation.

## Usage

``` r
default_params_doc(beast2_folder, has_internet, name, show_warnings, verbose)
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

- name:

  the package's name

- show_warnings:

  set to TRUE to show warnings

- verbose:

  set to TRUE for extra output, as can be used in debugging

## Note

This is an internal function, so it should be marked with `@noRd`. This
is not done, as this will disallow all functions to find the
documentation parameters

## Author

Richèl J.C. Bilderbeek
