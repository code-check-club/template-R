# Template project organisation for R code

This template is based on [Social Science Data Editors](https://social-science-data-editors.github.io/template_README/template-README.html) and is simplified for use with the [Code Review Guide](https://code-check-club.github.io/code-review-guide/).

Use this template to help you organize a project using R for for review. 

## Overview

Describe the project in general terms, but in enough detail for someone who is not familiar with it to be able to follow the code and understand what it is trying to accomplish.

## Data

All data used in this project come from built-in data in R, specifically the mtcars dataset of Motor Trend Car Road Tests (Henderson & Vellman, 1981).

Details of this dataset can be accessed in the help files in R (`?mtcars`). A machine-readable codebook in PsychDS format is included at data/mtcars.json.

## Computational Requirements

### Software Requirements

The code was compiled using R version >= 4.2, quarto 1.0.36, and the R packages:

* bookdown 0.28  
* knitr 1.39  
* quarto 1.2  
* rmarkdown 2.15  
* dplyr 1.0.9  
* ggplot2 3.3.6  
* kableExtra 1.3.4  
* readr 2.1.2  
* tidyr 1.2.0  

See [sessionInfo.txt](sessionInfo.txt) for further details.

``` r
# code to copy sessionInfo
sessionInfo() |> capture.output() |> write("sessionInfo.txt")
```

### Memory and Runtime Requirements

The code was last run on a 2017 iMac and took <1 minute to render.

## Instructions

Open the file appendixA.Rmd (R Markdown version) or appendixB.qmd (Quarto version) and knit/render using the interface in RStudio or the . All paths are relative, so no edits should be necessary. 

``` r
rmarkdown::render("appendixA.Rmd")
quarto::quarto_render("appendixB.qmd")
```

## Outputs

* [R Markdown](appendixA.html) or [Quarto](appendixB.html) appendix
* [Aggregated Data](data/aggregated.csv)
* [Figure 1](figures/plot1.png)
* [Table 1](tables/table1.html)

## References

* Henderson and Velleman (1981), Building multiple regression models interactively. Biometrics, 37, 391–411.

