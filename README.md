<p align="center">
  <img src="https://images.theconversation.com/files/209233/original/file-20180307-146694-aj4mc6.jpg?ixlib=rb-1.1.0&q=45&auto=format&w=1200&h=1200.0&fit=crop" alt="Sublime's custom image"
  width = 300
  height = 300 />
</p>

# Genderize
> Ptyhon & R version tool for `fetching genders of names` through the [genderize API](https://genderize.io/).


## Repository structure

* [Installations](https://github.com/Gmusebe/ACLED-Spatial-Analysis-with-R-#installations)
* [Setting Environment](https://github.com/Gmusebe/ACLED-Spatial-Analysis-with-R-#setting-environment)
* [Data](https://github.com/CodeForAfrica/genderize/tree/main/data)


## Installations
Install the latest release version of required packages from [CRAN](https://cran.r-project.org/web/packages/available_packages_by_name.html) with :

```R
install.packages(c('acled.api','dplyr', 'tibble', 'janitor', 'plotly', 'ggplot2'))

install.packages(c("sf", "leaflet", "leaflet.providers", "leaflet.opacity", "cartography"))
```

## Setting Environment
Call the library functions from the installed packages as follows:
> ACLED API
```R
library(acled.api)
```
> Tools for data manipulation feature engineering:
```R
library(dplyr)
library(tibble)
library(janitor)
```
> Summary visuals
```R
library(plotly)
library(ggplot2)
library(RColorBrewer)
```
>Spatial Analysis and Visuals
```R
library(sf)
library(tmap)
library(leaflet)
library(tmaptools)
library(cartography)
library(leaflet.opacity)
library(leaflet.providers)
```
### [Plotly Image Export](https://plotly.com/r/chart-studio-image-export/)
Using ``Plotly`` R package for summary visuals we would also want to save the static images.
Set the environment variables in the R session using ``Sys.setenv()``.
```R
Sys.setenv("plotly_username" = "Musebe")
Sys.setenv("plotly_api_key" = "*********")
```
## Data
Export ACLED data to R usin the ACLED API:

Sample view of the data:

| full_name  |
|-----------------|
|   Eli Daniels   |
|  Favour Peniel  |


## Copyright and license
The code structure has been sampled from [genderize.io](https://genderize.io/).