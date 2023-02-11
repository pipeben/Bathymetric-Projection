# Bathymetric-Projection
R-code that allows to project environmental ocean layers with depth dimension into only-bottom ocean layers to be used in Species Distribution Models (Useful for benthic species)

This is a simplyfied code with small example files that allow to run the R-codes to perform Bathymetric Projection on environmental
ocean variables with depth dimension (variables measured throughout the depth profile of the ocean)

The final product of BP is an ocean only-bottom layer appropriate to characterize benthic environments and use as predictor for Species 
Distribution Models for benthic species

Required Files
1. env_vars.nc = NetCdf file with variables chlorophyll-a (chl) and pH with monthly resolution throughout 25 depth classes (0.5 to 108.03 m depth)
    from 2015 to 2018 across the Colombian Pacific Ocean, with 0.25 spatial resolution.
    Source: Marine Copernicus product Global Ocean Biogeochemistry Hindcast "GLOBAL_MULTIYEAR_BCG_001_029" 
    https://data.marine.copernicus.eu/products 
    
2. bat.tif = Bathymetric layer for the Colombian Pacific Ocean with 0.016 spatial resolution
    Source: General Bathymetric Charts of the Oceans (GEBCO) with 0.08 spatial resolution
    
R-Code
The R code takes you through the six steps of BP described in Benavides et al (2023): 
"Improving spatiotemporal distribution models for marine shrimp species by appropriately projecting benthic environmental conditions"
It explains each GIS tool required for each step by using "env_vars.nc" and "bat.gif"

Resulting files
1.
2. 
   
