
<!-- README.md is generated from README.Rmd. Please edit that file -->

# audit

<!-- badges: start -->

[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
<!-- badges: end -->

An interactive application that ushers you through the inspection and
analysis of your growth curve experiments.

## Example

![alt text](eg.gif)

To start a new AUDIT session:

``` r
audit::run()
```

## Installation

Audit is currently only available on github and can be installed like
any other remote r package:

``` r
remotes::install_github("ggiaever/audit")
```

#### Step-by-step

1.  Install [R](https://cran.r-project.org) by downloading the
    appropriate package for your operating system from
    [cran](https://cran.r-project.org) and following the onscreen
    instructions.
2.  Install [Rstudio](https://www.rstudio.com/products/rstudio)
    (Optional), a development environment for R by downloading the
    appropriate image for your operating system from Rstudio’s [download
    page](https://www.rstudio.com/products/rstudio/download/#download)
    and follow the onscreen instructions.
3.  If this is a new R installation you will need to download some
    packages before being able to install audit. To do this, open R /
    Rstudio and enter the line below into the console. Follow the
    onscreen instructions.

<!-- end list -->

``` r
install.packages(c("devtools", "tidyverse", "remotes"))
```

4.  Install AUDIT and its dependencies by entering the line below into
    the console

<!-- end list -->

``` r
remotes::install_github("ggiaever/audit")
```

5.  To run AUDIT enter the line below at the console. This will open a
    new session in your default web browser.

<!-- end list -->

``` r
audit::run()
```

## More Info

### What is AUDIT?

AUDIT stands for **A**utomated **U**sher for **D**ata **I**nspection and
**T**idying (**AUDIT**). As in it helps you audit your growth curves.

AUDIT is really just an interactive interface to multiple modules. These
modules are also openly distributed as R packages:

  - [readcg12](https://github.com/npjc/readcg12)
  - [readgp1](https://github.com/npjc/readgp1)
  - [readyg](https://github.com/npjc/readyg)
  - [readbioscreen](https://github.com/npjc/readbioscreen)
  - [growr](https://github.com/npjc/growr)
  - [mtpview](https://github.com/npjc/mtpview) (and as a current
    workaround to known issue
    [mtpview1](https://github.com/npjc/mtpview1))

### If you find a bug

As you use AUDIT, if you find bugs, file an issue (ideally with a
reproducible example) at <https://github.com/npjc/audit/issues>. If you
are unsure how to make your example reproducible: provide input data
used and a description of the steps used or a link to a video
demonstrating it.

### Known Issue

The only change from previous communication is that mptview currently
exists as 2 separate packages (mptview and mtpivew1). This is a
temporary workaround for a bug in the underlying grid graphics system. I
will fold the mtpview1 back into the normal mtpview in the next R
release (grid is shipped with base R, more info).

### Experimental tag

The explore section is tagged as `experimental` as I will add new views
beyond what is already there. Once I have added all the views I will
remove the experimental tag.

### Additional Functionality Elsewhere

Earlier versions of this tool were used as prototypes and made
publically available through the [shinyapps.io](https://shinyapps.io)
service. These are still freely accesible via web browser (no
installation needed).

  - [cg12report](https://nicolascoutin.shinyapps.io/cg12report/)
    provides the ability to download a .pdf report of cg12 formatted
    data

  - [audit-lite](https://nicolascoutin.shinyapps.io/audit-lite/)
    provides interactive plate view where you can add reference line
    plots onto all wells of the plate (powered by [d3](https://d3js.org)
    via [r2d3](https://github.com/rstudio/r2d3)).

### Absolutely No Guarantees

I have tried my very hardest to ensure that the software performs as
intended. I use the same underlying tools for my own work. I however
make absolutely no guarantees about the use and or results of AUDIT and
its associated software. I therefore encourage you to validate your
assumptions and check your work.

### Alternatives and Prior Work

There are a number of other tools that may provide similar and/or other
useful functionality (in no particular order):

Interactive Applications:

  - [PROPHECY](http://prophecy.lundberg.gu.se/Main.aspx?Mainmnu=PRECOG):
    Described in <https://doi.org/10.1093/nar/gki126>
  - [PRECOG](http://precog.lundberg.gu.se/Pages/Content/Precog):
    Described in <https://doi.org/10.1186/s12859-016-1134-2>
  - [bgfit](http://sels.tecnico.ulisboa.pt/bgfit/): Described in
    <https://doi.org/10.1186/1471-2105-14-283>
  - [ACCESS](https://doi.org/10.1007/978-1-61779-173-4_15): Described in
    <https://doi.org/10.1007/978-1-61779-173-4_15>
  - [YODA](http://kaeberleinlab.org/yoda/): Described in
    <https://doi.org/10.1186/1471-2105-11-141>
  - [fitderiv](http://swainlab.bio.ed.ac.uk/software/fitderiv/):
    Described in <https://doi.org/10.1038/ncomms13766>

Software Packages:

  - [growthcurver](https://CRAN.R-project.org/package=growthcurver) R
    package
  - [plater](https://CRAN.R-project.org/package=plater) R package
  - [Colonyzer](https://doi.org/10.1186/1471-2105-11-287)
  - [agce](https://CRAN.R-project.org/package=agce) R package *ARCHIVED*
  - [drc](https://CRAN.R-project.org/package=drc) R package described in
    <https://doi.org/10.18637/jss.v012.i05>
  - [FitSearch](http://fitsearch.kaist.ac.kr) described in
    <https://doi.org/10.1186/1471-2164-14-S1-S6>
  - [getgrowth](https://pypi.org/project/getgrowth/) Python package
  - [grofit](https://CRAN.R-project.org/package=grofit) R package
    *ARCHIVED*, described in <https://doi.org/10.18637/jss.v033.i07>
  - [growcurves](https://CRAN.R-project.org/package=growcurves) R
    package, described in <https://doi.org/10.18637/jss.v057.i03>
  - [growthcurver](https://CRAN.R-project.org/package=growthcurver) R
    package, described in <https://doi.org/10.1186/s12859-016-1016-7>
  - [growthmodels](https://CRAN.R-project.org/package=growthmodels) R
    package
  - [pygrowthmodels](https://pypi.org/project/pygrowthmodels/) Python
    package
  - odelay described in <http://dx.doi.org/10.3791/4018>
