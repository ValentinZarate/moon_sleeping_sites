# Moon and capuchins sleeping sites

**Relation between sleeping site height of Black Capuchins (_Sapajus nigritus_) and Moon illumination**

This repository explores how lunar illumination and other environmental variables (e.g., Canopy hieght, NDVI, precipitation) influence sleeping site selection in wild Black Capuchin monkeys. The analysis combines GPS, moonlight, and remote sensing data to understand how primates may adaptively respond to night-time light conditions.

---

## Overview

- **Study species**: _Sapajus nigritus_ (Black Capuchin Monkey)
- **Location**: Iguazú National Park, Argentina
- **Key question**: Do Black Capuchins choose higher sleeping sites under darker lunar conditions?
- **Approach**: Combine spatial data (GPS), moonlight metrics (via `suncalc`), canopy height models, and precipitation data to evaluate behavioral patterns.

---
## HTML Reports

### Moon and Canopy height covariates
This section focuses on data cleaning, homogenization, and calculation of covariates. Here, we process and standardize the environmental data (such as moonlight and canopy height) that will later be used in the modeling steps.
The full report is available **[here](https://valentinzarate.github.io/moon_sleeping_sites/moon_sleeping.html)**.

### Buffer sizes and numbers of pseudo-absences
This section tests how different buffer sizes and numbers of pseudo-absence points influence the stability and reliability of the models. Choosing appropriate values is crucial to ensure robust inference and to minimize both statistical artifacts and spatial autocorrelation.
The full report is available **[here](https://valentinzarate.github.io/moon_sleeping_sites/moon_buffer_alternatives.html)**.

### Resource Selection Functions
Here we use Resource Selection Functions (RSF) to statistically evaluate the influence of moonlight, canopy height, and other covariates on the likelihood of sleeping site selection. RSFs allow us to estimate how much each factor contributes to site preference, accounting for the structure of the data (e.g., repeated measurements and grouping by night).
The full analysis and details are available **[here](https://valentinzarate.github.io/moon_sleeping_sites/rsf_moon.html)**.

It includes all figures, code, and ecological interpretations.

## Key R packages

- [`tidyverse`](https://www.tidyverse.org/) – data wrangling and plotting  
- [`suncalc`](https://cran.r-project.org/web/packages/suncalc/) – moon position and phase  
- [`terra`](https://rspatial.org/terra/) – raster data handling  
- [`geosphere`](https://cran.r-project.org/web/packages/geosphere/) – spatial distance and geometry  
- [`viridis`](https://cran.r-project.org/web/packages/viridis/) – color scales for accessibility  

## Structure
moon_sleeping_sites/
│
├── data/ # Raw data (not committed)
├── scripts/ # R scripts used in the analysis
├── output/ # Plots and figures
├── moon_sleeping.Rmd # Main analysis notebook
├── moon_sleeping.html # Rendered HTML report (published)
└── README.md # You are here

