# `fieldwalkr`: an R package for spatial sampling and field survey simulation
Joe Roe (University of Copenhagen)  
Presented at the Landscape Archaeology Conference, Newcastle & Durham, September 2018

This is the source repository for the above presentation. 
The slides are an interactive RMarkdown document using ioslides and shiny widgets.
You can view a live version at **https://joeroe.shinyapps.io/LAC2018_fieldwalkr/**.
Alternatively, the slides can be run locally using RStudio; see instructions below.

## Abstract

Recent efforts to promote reproducibility in archaeology have focused primarily on data analysis and dissemination. However, open science begins earlier, with a transparent experimental design and well-defined data collection protocol. The ‘experiments’ performed by archaeologists—field investigations and physical analyses of unique objects—are rarely actually repeatable. However, the reproducibility of particular results in similar archaeological contexts is still strongly affected by choices made in the field, such as where and how to survey or excavate, and what sampling strategy to use. In this session, I will demonstrate `fieldwalkr`, an R package for simulating spatial sampling that I developed to try and address some of these issues in archaeological surveys. The package includes tools for modelling the effect of different sampling strategies, survey parameters, and detection functions on the estimation of spatial point patterns. The target distributions can either be generated from a variety of null models or extrapolated from real archaeological landscapes. Its aim is to facilitate more informed and statistically rigorous survey design, as well as provide a framework for post-hoc and theoretical analyses of sampling effects. A shiny web interface makes it accessible for exploratory use and in the classroom, whilst the underlying package can be used to document the research design process as an open, reproducible R script.

## Run slides locally via RStudio

To view the slides locally, you will first need to clone or download this repository, and make you have all the following packages are installed:

```{r}
# fieldwalkr package
devtools::install_github("joeroe/fieldwalkr")

# CRAN dependencies
install.packages(c("tidyverse", "magrittr", "sf", "maptools", "RandomFields", "RandomFieldsUtils", "spatstat"))
```

Then simply open `Roe_fieldwalkr_slides.Rmd` in RStudio and click "Run Presentation" above the editing window.
RStudio will knit the document and start a local server to view it.
