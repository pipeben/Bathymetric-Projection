#Bathymetric-Projection

(Note: You might also be interested in the Bathymetric Projection code https://github.com/pipeben/Bathymetric-Projection)

This is an R-code that implements the Bathymetric Projection Method (BP). 
This method allows to project environmental ocean layers with depth dimension (measured or modeled throughout the ocean profile depth at different depths or depth classes) into bottom ocean layers. The bottom layers produced by the BP method are useful as predictors for Species Distribution Models 
for benthic species

We provide a reproducible example including R-code and small files that allow to easily run and understand BP on environmental
ocean variables with depth dimension

REQUIRED FILES
1. ‘env_vars.nc’ = NetCdf file with variables chlorophyll-a (chl) and pH with monthly resolution throughout 25 depth classes (0.5 to 108.03 m depth)
    Time span from 2015 to 2018. Spatial extent across the Colombian Pacific Ocean, with 0.25°resolution.
    Source: Marine Copernicus product Global Ocean Biogeochemistry Hindcast "GLOBAL_MULTIYEAR_BCG_001_029" 
    https://data.marine.copernicus.eu/products 
    
2. ‘bat.tif’ = Bathymetric layer for the Colombian Pacific Ocean with 0.016 spatial resolution
    Source: General Bathymetric Charts of the Oceans (GEBCO)
    https://www.gebco.net/ 
    
3. R-CODE
    The file ‘Rcode_BP.R’ takes you through the six steps of BP described in Benavides et al (2023) 
    It explains each geospatial and statistic tool required during each step using ‘env_vars.nc’ and ‘bat.gif’ within a simplified example


RESULTING FILES
1. ‘chl_bottom_jan.tif’ = Ocean bottom layer for variable chlorophyll in January resulting after BP processing

2. ph_bottom_jan.tif = Ocean bottom layer for variable ph in January resulting after BP processing

3. my_bottom_layers.tif = files "chl_bottom_jan.tif" and "ph_bottom_jan.tif" stacked and saved into a new raster tif


NOTES
1. As a simplified example this code produces ocean bottom layers for chl and ph during january

2. You can just replace name "jan" by "feb" or any months’ abbreviation in the code to obtain ocean bottom layers for each month

3. As a simplified example this code produces ocean bottom layers for chl and ph during janary across the Colombian Pacific Ocean throughout 25 depth classes (0.5 to 108.03 m). You can produce ocean bottom layers for any ocean variable, trough any set of depth classes, across any oceanic area in the world and, also with different spatial and temporal (y-m-d) resolutions as long as the original data allows it.

***THANK YOU FOR USING BATHYMETRIC PROJECTION FOR YOUR RESEARCH***
If you have any questions please write to pipeben@gmail.com 
