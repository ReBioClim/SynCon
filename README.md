# SynCon

A decision-support tool to identify synergies and conflicts between spatial conditions and public support for urban stream restoration.

[![DOI: 10.5281/zenodo.23370008](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.23370008-blue)](https://doi.org/10.5281/zenodo.23370008) [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE) [![Rbanism: R package](https://img.shields.io/static/v1?label=Rbanism&message=R%20package&labelColor=93278F&color=00A99D&style=flat-square)](https://github.com/Rbanism)

[Launch SynCon — latest version](https://rebioclim.shinyapps.io/SynCon-202610/)

SynCon is an interactive R Shiny application that compares spatial conditions and public support for identified ecological restoration goals. It acts as a decision-support tool, helping city planners, restoration teams and researchers explore where restoration measures align with public preferences and where further stakeholder engagement or restoration measures may be needed.

The tool follows the ReBioClim Deliverable [D1.3.1](https://www.interreg-central.eu/wp-content/uploads/2026/09/D1.3.1-ReBioClim-Synergies-And-Conflicts.pdf) workflow for social-ecological synergies and conflicts. Data from four ReBioClim pilot streams, Bila Nisa, Geberbach, Piasnica and Teplica, illustrate the method.

## How to use this tool

Follow the four steps in the app:

1.  **Restoration Measures:** review the measures and associated indicators.
2.  **Spatial Data:** download and complete the spatial-data table using the provided scoring guidance.
3.  **Public Support:** download and complete the public-support table using survey evidence.
4.  **SynCon Results:** upload the completed tables, or paste standardized spatial-condition and public-support scores from 1 to 5, then calculate the results.

The **ReBioClim Example** tab provides a worked example, and the **Help** tab explains the input requirements. Results support interpretation and discussion; local site assessment and stakeholder engagement remain necessary when planning restoration.

## Run locally

Install [R](https://www.r-project.org/) version 4.1 or later. Clone this repository:

``` sh
git clone https://github.com/ReBioClim/SynCon.git
```

Install the required R packages:

``` r
install.packages(c(
  "shiny", "sf", "leaflet", "DT", "bslib", "dplyr",
  "ggplot2", "ggrepel", "plotly"
))
```

Run the application from the repository root, where `app.R` is located:

``` r
shiny::runApp(".")
```

Keep the accompanying files (csv, gpkg, css, png) in their original locations.

## Citation

If you use SynCon in your research, please cite the archived version you used. For version 0.1.0:

> Wu, Y., & Forgaci, C. (2026). *SynCon: Synergies and Conflicts analysis for urban stream restoration* (v0.1.0) [Software]. Zenodo. <https://doi.org/10.5281/zenodo.23370008>

## Project and contributions

SynCon is developed by Yehan Wu and Claudiu Forgaci at Delft University of Technology as part of [ReBioClim](https://www.interreg-central.eu/projects/rebioclim/).

Please report bugs or suggest improvements through [GitHub Issues](https://github.com/ReBioClim/SynCon/issues).
