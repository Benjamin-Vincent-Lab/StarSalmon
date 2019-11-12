Post processes output from the star salmon pipeline.

## Example
``` r
StarSalmon::post_process_star_salmon(
  input_file_paths = input_file_paths,
  output_dir = star_salmon_dir,
  sample_data_path = sample_data_path,
  thread_num = thread_num,
  sample_folder_column = "run_accession"
  )
```

## Assembling this package
In R:
``` r
housekeeping::assemble_package(package_name = "StarSalmon", my_version = "0.0-14",
  my_dir = "/datastore/alldata/shiny-server/rstudio-common/dbortone/packages/StarSalmon")
```

## Push changes
In bash:
``` bash
cd /datastore/alldata/shiny-server/rstudio-common/dbortone/packages/StarSalmon
my_comment="Removed packages from import statement."
git commit -am "$my_comment"; git push origin master
git tag -a 0.0-14 -m "$my_comment"; git push -u origin --tags
```

## Install
Restart R
In R (local library, packrat library):
``` r
devtools::install_github("Benjamin-Vincent-Lab/StarSalmon")
```

Or for a specific version:
``` r
devtools::install_gitlab("Benjamin-Vincent-Lab/StarSalmon", ref = "0.0-14")
```

## Previous locations
https://sc.unc.edu/dbortone/starsalmon
https://sc.unc.edu/benjamin-vincent-lab/starsalmon
Moved to github so that the package could be accessed without a token.
