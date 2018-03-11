# Installation of OpenAlea environment and R

## Installation of OpenAlea

### Conda Installation

[Conda](https://conda.io) is a package manager that can be installed on Linux, Windows, and Mac.
If you have not yet installed conda on your computer, follow these instructions:

[Conda Installation](https://conda.io/docs/user-guide/install/index.html)

#### Windows, Linux, Mac

Create an environment named *openalea*:

    conda create -n openalea -c openalea openalea.plantgl openalea.lpy

Activate the *openalea* environment:

    [source] activate openalea

Install the different packages

    conda install -c openalea openalea.mtg alinea.caribu plantscan3d openalea.visualea

    conda install -c openalea -c conda-forge python-pvlib alinea.astk

## Installation of R & co

You can install everythong by yourself, or use the r channel in conda

### Install RStudio, Rmarkdown

[source] deactivate
conda create -n renv -c r rstudio r-rmarkdown

### Install R packages
* PerformanceAnalytics
* lme4
* car
* agricolae
* sensitivity
* lhs
* planor

Under **R**, you can install everything using
  install.packages(c('PerformanceAnalytics','lme4','car','agricolae','sensitivity','lhs','planor') )

