# Moon and capuchins sleeping sites

**Relation between sleeping site height of Black Capuchins (_Sapajus nigritus_) and Moon illumination**

This repository explores how lunar illumination and other environmental variables (e.g. precipitation, canopy structure) influence sleeping site selection in wild Black Capuchin monkeys. The analysis combines GPS data, lunar ephemerides, and remote sensing to investigate how primates may adaptively respond to night-time light conditions.

---

## Overview

- **Study species**: _Sapajus nigritus_ (Black Capuchin Monkey)
- **Location**: Iguazú National Park, Argentina
- **Key question**: Do Black Capuchins choose higher sleeping sites under darker lunar conditions?
- **Approach**: Combine spatial data (GPS), moonlight metrics (via `suncalc`), canopy height models, and precipitation data to evaluate behavioral patterns.

---

## Highlights

- Calculates **effective moonlight index**:  
  Combines moon phase and altitude to estimate true perceived nocturnal illumination.

- Integrates **canopy structure data** from remote sensing (Lidar-based CHM).

- Links **sleeping site use (used vs. available points)** to moonlight, canopy height, and precipitation.

- Produces **interactive plots** and **static figures** via R and `ggplot2`.

---

## HTML Report

The full HTML report is available **[Here](https://valentinzarate.github.io/moon_sleeping_sites/moon_sleeping.html)**

It includes all figures, code, and ecological interpretations.

## Key R packages

- [`tidyverse`](https://www.tidyverse.org/) – data wrangling and plotting  
- [`suncalc`](https://cran.r-project.org/web/packages/suncalc/) – moon position and phase  
- [`terra`](https://rspatial.org/terra/) – raster data handling  
- [`geosphere`](https://cran.r-project.org/web/packages/geosphere/) – spatial distance and geometry  
- [`viridis`](https://cran.r-project.org/web/packages/viridis/) – color scales for accessibility  

## 📁 Structure
moon_sleeping_sites/
│
├── data/ # Raw data (not committed)
├── scripts/ # R scripts used in the analysis
├── output/ # Plots and figures
├── moon_sleeping.Rmd # Main analysis notebook
├── moon_sleeping.html # Rendered HTML report (published)
└── README.md # You are here

