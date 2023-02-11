# Bathymetric-Projection
R-code that allows to project environmental ocean layers with depth dimension into only-bottom ocean layers to be used in Species Distribution Models (Useful for benthic species)

This is a simplyfied code with small example files that allow to run the R-codes to perform Bathymetric Projection on environmental
ocean variables with depth dimension (variables measured throughout the depth profile of the ocean)

The final product of BP is an ocean only-bottom layer appropriate to characterize benthic environments and use as predictor for Species 
Distribution Models for benthic species

REQUIRED FILES
1. env_vars.nc = NetCdf file with variables chlorophyll-a (chl) and pH with monthly resolution throughout 25 depth classes (0.5 to 108.03 m depth)
    from 2015 to 2018 across the Colombian Pacific Ocean, with 0.25 spatial resolution.
    Source: Marine Copernicus product Global Ocean Biogeochemistry Hindcast "GLOBAL_MULTIYEAR_BCG_001_029" 
    https://data.marine.copernicus.eu/products 
    
2. bat.tif = Bathymetric layer for the Colombian Pacific Ocean with 0.016 spatial resolution
    Source: General Bathymetric Charts of the Oceans (GEBCO) with 0.08 spatial resolution 
    https://www.gebco.net/ 
    
R-CODE
The Rcode_BP.R takes you through the six steps of BP described in Benavides et al (2023): 
"Improving spatiotemporal distribution models for marine shrimp species by appropriately projecting benthic environmental conditions"
It explains each GIS tool required during each step using "env_vars.nc" and "bat.gif" within a simplified example

RESULTING FILES
1. chl_bottom_jan.tif = Ocean only-bottom layer for variable chlorophyll in January resulting after BP processes 
2. ph_bottom_jan.tif = Ocean only-bottom layer for variable ph in January resulting after BP processes 
3. my_bottom_layers.tif = files "chl_bottom_jan.tif" and "ph_bottom_jan.tif" stacked and saved into a new raster tif

NOTES
1. 
   
