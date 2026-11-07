# EDS223 HW3: Marine Aquaculture Potential in the U.S. West Coast Exclusive Economic Zones

<img width="740" height="555" alt="geoduck" src="https://github.com/user-attachments/assets/c1436620-1357-4646-931d-4a241f273ee5" />


## Purpose
This repository analyzes the suitability of marine aquaculture development within the U.S. West Coast Exclusive Economic Zones (EEZ). This analysis uses geospatial data and environmental constraints of sea surface temperature (SST) and water depth for species-specific habitat requirements to help identify areas with high aquaculture potential. The analysis specifically looks at Oysters and Pacific Geoducks. This research is motivated by highlighting that maximizing marine aquaculture potential could help meet growing global seafood demand.

## Overview
Highlights:
- hw3.qmd file: The first section contains code to identify the greatest marine aquaculture potential in the U.S. West Coast Exclusive Economic Zones, this includes data cleaning, matching resolution, extent, and CRS of the spatial datasets. The code is refined into a function to easily find the the greatest marine aquaculture potential in the U.S. West Coast Exclusive Economic Zones for other marine species. 
- Data folder: houses the spatial average annual sst data spanning from 2009-2012, depth.tif (spacial data), and wc_regions_clean vector spatial data of the  West Coast Exclusive Economic Zones.

```{r}
EDS-223-Marine-Aquaculture-Potential-in-U.S.-West-Coast-Exclusive-Economic-Zones
└───data
     └───average_annual_sst_2008.tif
         average_annual_sst_2009.tif
         average_annual_sst_2010.tif
         average_annual_sst_2011.tif
         average_annual_sst_2012.tif
         depth.tif
         wc_regions_clean.dbf
         wc_regions_clean.prj
         wc_regions_clean.shp
         wc_regions_clean.shx
│   hw3.pdf
│   hw3.qmd
│   README.md
```

## Data Access
The SST data was originally generated from NOAA’s 5km Daily Global Satellite Sea Surface Temperature Anomaly v3.1. The datasets used in this analysis was obtained from a downloadable data folder provided through the Environmental Data Science 223 course at the University of California of Santa Barbara website by Annie Adams: https://eds-223-geospatial.github.io/assignments/HW3.html. 

Bathymetry dataset characterizes the depth of the ocean from the General Bathymetric Chart of the Oceans (GEBCO). This dataset was obtained from a downloadable data folder provided through the Environmental Data Science 223 course at the University of California of Santa Barbara website by Annie Adams: https://eds-223-geospatial.github.io/assignments/HW3.html. 

The HOLC Grade data originally came from a team of researchers at the University of Richmond that digitized maps and information from the HOLC as part of the Mapping Inequality project: https://dsl.richmond.edu/panorama/redlining/#loc=5/39.1/-94.58. For this project specifically we will be working with maps of HOLC grade designations for Los Angeles, CA. This dataset used in this analysis was obtained from a downloadable data folder provided through the Environmental Data Science 223 course at the University of California of Santa Barbara website by Annie Adams: https://eds-223-geospatial.github.io/assignments/HW3.html. 

The Exclusive Economic Zones dataset is spatial dataset used to define the maritime boundaries using Exclusive Economic Zones off of the west coast of US from Marineregions.org. The Crashes data comes from the Statewide Integrated Traffice Records System (SWITRS) database collects and processes data gathered from a collision scenes. This dataset used in this analysis was obtained from a downloadable data folder provided through the Environmental Data Science 223 course at the University of California of Santa Barbara website by Annie Adams: https://eds-223-geospatial.github.io/assignments/HW3.html. 

## Author
Nina Berry: https://github.com/nberry18 

## References
- Average annual sea surface temperature (SST) from the years 2008 to 2012: average annual dataset: https://coralreefwatch.noaa.gov/product/5km/index_5km_ssta.php
- Ocean depth dataset: https://www.gebco.net/data_and_products/gridded_bathymetry_data/#area
- Exclusive Econonic Zones dataset: https://www.marineregions.org/eez.php
- 223 Homework 3 assignment description: https://eds-223-geospatial.github.io/assignments/HW3.html
