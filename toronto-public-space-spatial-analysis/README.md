# Spatial Analysis of Public Spaces in Toronto

## Project Overview

This project investigates the spatial distribution of public spaces and parks across Toronto neighbourhoods and explores potential relationships between public space availability and socioeconomic characteristics.

The analysis examines whether public spaces are distributed equitably across neighbourhoods with different socioeconomic profiles, with a particular focus on median family income, population size, unemployment, and child population.

Geographic information systems (GIS), spatial statistics, and statistical modelling techniques are used to identify spatial patterns, assess clustering, and investigate factors associated with the distribution of public spaces.

## Research Objectives

- Examine the geographic distribution of parks and public recreation facilities across Toronto.
- Investigate the relationship between neighbourhood socioeconomic characteristics and public space availability.
- Assess whether lower-income neighbourhoods have comparatively limited access to public spaces.
- Identify spatial clustering and patterns in the distribution of public spaces.
- Evaluate the influence of demographic and socioeconomic variables on public space distribution using statistical and spatial regression models.

## Data Sources

The project uses three primary datasets:

1. **Parks and Recreation Facilities:** Geographic locations of public spaces and recreation facilities across Toronto.
2. **Toronto Neighbourhood Boundaries:** Geographic boundaries used to conduct neighbourhood-level spatial analysis.
3. **Toronto Neighbourhood Statistics:** Socioeconomic and demographic information, including median family income, unemployment rates, total population, and child population.

The datasets are integrated using spatial joins and neighbourhood-level geographic identifiers.

## Methodology

The project employs several spatial and statistical analytical techniques.

### 1. Exploratory Spatial Analysis

- Geographic mapping of Toronto neighbourhoods using median family income.
- Visualization of public space locations across the city.
- Comparison of public space counts across neighbourhoods.
- Calculation of public spaces per 1,000 residents and public spaces per child.

### 2. Spatial Autocorrelation

- Moran's I to evaluate spatial autocorrelation in public space distribution.
- Queen contiguity spatial weights.
- Spatial correlograms to investigate spatial clustering across neighbourhoods.

### 3. Statistical and Spatial Regression

- Multiple Linear Regression to examine relationships between public space counts and socioeconomic and demographic characteristics.
- Spatial Autoregressive Error (SAR) modelling to account for spatial dependencies.
- Residual spatial autocorrelation testing to assess model performance.

### 4. Point Pattern Analysis

Spatial point pattern methods are used to investigate the geographic distribution and density of public spaces.

Techniques include:
- Kernel Density Estimation.
- Poisson Point Process Models.
- Ripley's K-function.
- G-function and nearest-neighbour analysis.
- Quadrat analysis.
- Dirichlet tessellation.

### 5. Spatial Clustering

DBSCAN clustering is used to identify geographic clusters of public spaces.

### 6. Count Regression

Poisson regression is applied to investigate the relationship between public space counts and neighbourhood-level socioeconomic and demographic characteristics.

## Key Findings

- Public spaces are not uniformly distributed across Toronto, with noticeable geographic concentrations in certain areas.
- Neighbourhood-level public space counts vary considerably across the city.
- Normalizing public space counts by population provides a different perspective on neighbourhood-level accessibility.
- Moran's I analysis identifies statistically significant, albeit weak, positive spatial autocorrelation in park counts (I = 0.0737, p = 0.0488).
- Linear regression suggests that neighbourhood area, total population, and child population are positively associated with park counts.
- Median family income does not demonstrate a statistically significant relationship with park counts in the initial linear regression.
- The spatial error model accounts for spatial dependence, with residual Moran's I testing indicating no statistically significant remaining spatial autocorrelation (p = 0.4601).

These findings highlight the importance of considering spatial context, population characteristics, and neighbourhood-level differences when examining equitable access to public spaces.

## Tools and Technologies

- R
- R Markdown
- Tidyverse
- SF (Simple Features)
- Leaflet
- ggplot2
- spdep
- spatialreg
- spatstat
- DBSCAN

## Repository Structure

```text
toronto-public-space-spatial-analysis/
│
├── README.md
├── data/
│   └── Green Spaces - 4326
|       └── <Associated Files>
│   ├── Parks and Recreation Facilities - 4326
|       └── <Associated Files>
│   └── Toronto Neighbourhoods
|       └──<Associated Files>
└── toronto_public_space_analysis.Rmd
```

## Limitations and Future Research

The analysis is based on neighbourhood-level data and public space locations, which may not fully capture actual accessibility or quality of public spaces.

Future research could incorporate additional accessibility measures, including walking distance, public transportation availability, park size, facility quality, and population density.

Further investigation could also explore spatial relationships between socioeconomic characteristics and public space accessibility using more comprehensive spatial econometric models.

## References

- City of Toronto – Parks and Recreation Facilities data.
- City of Toronto – Neighbourhood boundaries and neighbourhood statistics.

