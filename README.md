# training-rstudio-binder

This repository holds binder files to create an Rstudio binder that can be used for training events.

**For CFDE trainers:** if you'd like to build a new Rstudio binder with other installations from this repo - 

1) create a new branch
2) edit `environment.yml` file in the [./binder](./binder) directory
3) build a [new pangeo binder](https://binder.pangeo.io/)

![](./rstudio-binder-setup.png)

4) add the binder badge + brief description to this readme doc (including the repo branch)

**Important reminders:**

- `r-base` needs to be in the `environment.yml` file so that R is installed
- in the pangeo binder form:
  - specify Github branch to point binder to
  - change "Path to a notebook file (optional)" dropdown to "URL" from "File". Type `rstudio` so the binder opens Rstudio.
- do not merge branches to `main` or delete branches that existing binders are pointing to, otherwise those binders will not work anymore!

## Binders

This binder (on `basic-rstudio`) only has R installed:

[![Binder](https://binder.pangeo.io/badge_logo.svg)](https://binder.pangeo.io/v2/gh/nih-cfde/training-rstudio-binder/basic-rstudio?urlpath=rstudio)


