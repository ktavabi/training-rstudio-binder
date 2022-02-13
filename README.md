# training-rstudio-binder

This repository holds binder files to create an Rstudio binder that can be used for training events.

## Binders


- [![Binder](https://mybinder.org/badge_logo.svg)](https://binder.pangeo.io/v2/gh/nih-cfde/training-rstudio-binder/basic-rstudio?urlpath=rstudio) The binder on the  `basic-rstudio` branch only has R installed:

- [![Binder](https://mybinder.org/badge_logo.svg)](https://binder.pangeo.io/v2/gh/nih-cfde/training-rstudio-binder/rstudio-snakemake-workflow?urlpath=rstudio) The binder on the `rstudio-snakemake-workflow` branch has R, snakemake-minimal, and some variant calling software.

- [![Binder](https://mybinder.org/badge_logo.svg)](https://binder.pangeo.io/v2/gh/nih-cfde/training-rstudio-binder/conda-workshop-march2021?urlpath=rstudio)
 The binder on the `conda-workshop-march2021` branch has Rstudio and example code files for conda workshop.

- [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nih-cfde/training-rstudio-binder/data?urlpath=rstudio) The binder on the `data` branch has all the data files used in UNIX workshops

- [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nih-cfde/training-rstudio-binder/recount3?urlpath=rstudio) The binder on the `recount3` branch has many R packages from CRAN and Bioconductor


## Adding new binders *from this repo*

**For CFDE trainers:** if you'd like to build a new Rstudio binder with other installations from this repo - 

1) create a new branch
2) edit `environment.yml` file in the [./binder](./binder) directory
3) build a [new pangeo binder](https://binder.pangeo.io/) - remember to enter the correct Github branch!

![](./rstudio-binder-setup.png)

4) add the binder badge + brief description to this readme doc (including the repo branch)

**Important reminders:**

- `r-base` or some r package (e.g., `r-ggplot2`) needs to be in the `environment.yml` file so that R is installed during binder build
- in the pangeo binder form:
  - specify Github branch to point binder to
  - change "Path to a notebook file (optional)" dropdown to "URL" from "File". Type `rstudio` so the binder opens Rstudio.
- do not merge branches to `main` or delete branches that existing binders are pointing to, otherwise those binders will not work anymore!

