# Moon and capuchins sleeping sites

**Relation between sleeping site height of Black Capuchins (_Sapajus nigritus_) and Moon illumination**

This repository explores how lunar illumination and other environmental variables (e.g. precipitation, canopy structure) influence sleeping site selection in wild Black Capuchin monkeys. The analysis combines GPS data, lunar ephemerides, and remote sensing to investigate how primates may adaptively respond to night-time light conditions.

---

## Overview

- **Study species**: Black Capuchin Monkey (_Sapajus nigritus_)
- **Location**: Iguazú National Park, Argentina
- **Key question**: Does moonlight modulate sleeping site selection in a diurnal primate?
- **Approach**: Combine spatial data (GPS), moonlight metrics (via `suncalc`), canopy height and density (NDVI) models (LiDAR and remote sensing; [Lang et al. 2022](https://www.nature.com/articles/s41559-023-02206-6)), and climate data to evaluate sleeping site patterns.

---

## Codes

### Moon and Canopy covariates
The full code and details are available **[here](https://valentinzarate.github.io/moon_sleeping_sites/moon_sleeping.html)**.

### Buffer sizes and numbers of pseudo-absences
The full code and details are available **[here](https://valentinzarate.github.io/moon_sleeping_sites/moon_buffer_alternatives.html)**.

### Resource Selection Functions
The full code and details are available **[here](https://valentinzarate.github.io/moon_sleeping_sites/rsf_moon.html)**.

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
├── moon_sleeping_buffers.html # Rendered HTML report (published)
├── rsf.html # Rendered HTML report (published)
└── README.md # You are here
