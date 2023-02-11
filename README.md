# Bathymetric-Projection
R-code that allows to project environmental ocean layers with depth dimension into only-bottom ocean layers to be used in Species Distribution Models (Useful for benthic species)

This is a simplyfied code with small example files that allow to run the R-codes to perform Bathymetric Projection on environmental
ocean variables with depth dimension (variables measured throughout the depth profile of the ocean)

The final product of BP is an ocean only-bottom layer appropriate to characterize benthic environments and use as predictor for Species 
Distribution Models for benthic species

Required Files
1. env_vars.nc = NetCdf file with variablse chlorophyll-a (chl) and pH measured monthly throughout 25 depth classes (0.5 to 108.03 m depth)
