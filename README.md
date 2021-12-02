<!-- README.md is generated from README.Rmd. Please edit that file -->

# Welcome to the NHS-R Community Introduction to R and R Studio! <a alt="NHS-R Community's logo" href='https://nhsrcommunity.com/'><img src='https://nhs-r-community.github.io/assets/logo/nhsr-logo.png' align="right" height="80" /></a>

<!-- badges: start -->
<!-- badges: end -->

## Attending the course?

If you are attending the course all the course materials and preparation
instructions are
[here](https://philosopher-analyst.netlify.app/collection/nhsr-intro/prework/).

## Are you wanting to update or use the slide code?

This repository is split into 3 areas:

-   [RMarkdown files and dependency
    files](https://github.com/nhs-r-community/intro_r/tree/main) -
    slides have been built in {xaringan} which requires the css, img and
    libs folder to render
-   [html
    pages](https://github.com/nhs-r-community/intro_r/tree/gh-pages) -
    are automatically rendered using GitHub actions (no need to knit
    every file!) and are kept on a separate branch. The html files are
    published though GitHub
    [here](https://nhs-r-community.github.io/intro_r/) and being
    {xaringan} they are interactive and accessible
-   [data
    files](https://github.com/nhs-r-community/intro_r_data/tree/26a2e39bd49d4aa95a8efc5b45c398386e6e4ed4)
    are in a separate repository to help learners access the data files
    separate to the code for the slides

## Cloning this repository

Note that the following code is used in the `Terminal` not in R!

The [data/](https://github.com/nhs-r-community/intro_r_data/) folder is
a submodule, in order to properly clone this repository you should run
the following:

``` sh
git clone --recurse-submodules https://github.com/nhs-r-community/intro_r.git
```

Alternatively, if you have already cloned the repository locally, you
can run the following to load the
[data/](https://github.com/nhs-r-community/intro_r_data/) submodule:

``` sh
git submodule init
git submodule update
```

## Packages used

The slides have been built using {xaringan} and you’ll need to install
the following packages:

``` r
install.packages("tidyverse", "xaringan", "kableExtra", "magick", "NHSRdatasets", "rmarkdown", "callr", "withr", "fs", "here")
devtools::install_github("gadenbuie/xaringanExtra", "nhs-r-community/nhsrtheme", "mitchelloharawild/icons")
```

If you have forked and/or cloned this repository you can install all of
the required packages to run this project with the following:

``` r
devtools::install_deps(dependencies = TRUE)
```

## Spotted a mistake?

Please let us know if there are mistakes or improvements by creating an
[issue](https://github.com/nhs-r-community/intro_r/issues).
