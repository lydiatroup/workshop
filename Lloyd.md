
## HIGH RESOLUTION GLOBAL GRIDDED DATA FOR USE IN POPULATION STUDIES

# definitions
scale is the area the dataset covers
disaggregation is the breaking down of data into smaller categories, in this case into administrative boundaries
adminsrative areas are the ways a country is broken up into smaller municipalities with different levels of control / authority
grid cells / rasters
uniform distribution / proportional allocation: uses the assumption that the population of a grid cell is an exclusive function of land area in that grid cell

The authors use a variety of datasets in their methadology making it better than a conventional census. They used multiple datasets for each data type, with 
different sources, years, and spatial resolutions.
Because of the multitude of datasets used, WorldPop can be updated more often than a traditional census and may contain a greater variety of information. 
Additionally, this dataset has linked attribute data to spatial locations, which traditional census typically does not do. Census data, at least United States
Census data is typically presented through spreadsheets, which the authors linked to administrative boundaries. This means the vector data of administrative 
boundaries has gained the attribute data the census datasets have provided.
This was accomplished using arcgis and qgis software to join spatial data to attribute data. 



# notes
areal-weighing approach
    - disaggregate population from census units into grid cells through the simple assumption that the population of a grid cell is an exclusive function of the land area within that pixel
    - precision and accuracy varies based on size on input unit
    
anciallary spatial data 
    - combines census data with urban extents mapped from sattalites
    
    world pop -> random forest model. combines census data and open access data sets from remotely senses and geospatial datasets, then uses random forests model to make a gridded prediction of population density. 
    
    4 base standardized 100 m tiled datasets and 30 arcsecond global mosaic derivates (1km datasets)
    
    - base dataset creation = process raster topography data with vector country boundary data via gis
        4 main 100m resolution datasets (topography, standardised, gridded, clipped to country coastal boundaries)
        
        topography data: Vieewfinder panoramas dataset (US NASA info + SRTM)
        country boundary data: GADM (not geoboundaries rip) (new beta version uses new country boundaries based on CIESIN instead of GADM)
        GDAL > arc for processing large raster datasets
        also uses qgis for open street map data
        
        this is so cool i love gis tis fun
        
        there are some issues still because of inconsistencies in the data used but not too bad
        
