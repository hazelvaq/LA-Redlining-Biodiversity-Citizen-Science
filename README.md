# Investigating Historical Redlinings Impacts on Citizen Scientist reported Bird Observations
![image](https://github.com/hazelvaq/LA-Redlining-Biodiversity-Citizen-Science/assets/108312152/c8121288-e200-4d8b-abba-6ff813f1a1e7)


[*LA County Historical Redlining*](https://pbssocal.org/shows/lost-la/segregation-in-the-city-of-angels-a-1939-map-of-housing-inequality-in-l-a)

## About 

This repo contains an Rmarkdown `redlining_biodiversity.Rmd`, that analysis how historical redlining in LA county display modern day consequences 
on health, economic development, and biodiversity. This project explores if historical redlining has an affect on reported bird observations from citizen scientist. 
Are "low" grade neighborhoods in LA are reporting less bird observations than their counterpart "higher" grade neighborhoods?

Steps taken to analyze:
Spatial files were analyzed using `sf` package
1. Import data files using `sf` package
2. Prepare raster data for manipulation
3. Map LA county environmental justice parameters
4. Spatially join historical raster map and EJScreen data
5. Summarize bird observations for the different neighborhood grades in Redlining 

## Data Citations
Data was obtained from:
[EPA EJScreen](https://ejscreen.epa.gov/mapper/)
[Digital Scholarship Lab](https://dsl.richmond.edu/)
[Global Biodiversity Information Facility](gbif.org)

## File Structure
```bash
├── data
│   ├── EJSCREEN_2023_BG_StatePct_with_AS_CNMI_GU_VI.gdb
│   └── gbif-birds-LA
│       ├── gbif-birds-LA.dbf
│       ├── gbif-birds-LA.prj
│       ├── gbif-birds-LA.shp
│       └── gbif-birds-LA.shx
├── LA-Redlining-Biodiversity-Citizen-Science.Rproj
├── README.md
├── redlining_biodiversity.html
└── redlining_biodiversity.Rmd
```
