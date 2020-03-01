Geospatial data aggregation: cases &amp; examples
=======
### Myeong Lee
----


### 0. Getting Ready
* This tutorial is based on [R](https://www.r-project.org/).
* Sample data is available in the `data` folder (a sample of Car2Go's location data)
* Sample code is availalbe at the `.Rmd` files.
* Currently, there are two sample files available (`geo_agg_tutorial.Rmd` for geospatial visualization and aggregation; and `voronoi_overlay_sample.Rmd` for generating Voronoi diagram based on real-world points).
	 
### 1. Geospatial Points 
* Loading the data as a dataframe (if lon/lat).
* Loading the data as SpatialPointsDataFrame (`sp` package).

### 2. Geospatial Polygons
* Sources might be `GeoJSON`, `Shapefile`, or `KML`. 
* Loading the data as SpatialPolygonDataFrame (`sp` package). 
* Many boundaries datasets available from Census or city data portals.

### 3. Basic Geospatial Operations
* `raster` package for intersection, union, and etc. 
* It's possible to iterate through each polygon in a SpatialPolygonDataFrame. 
* Example: Aggregation I: Points to Polygons

### 4. Density-based Viz
* Using `ggplot` and `ggmap` to visualize frequency using the color gradiation (polygon-based).

### 5. Generating Polygons
* Hexagons (in this example)
* Grids
* Voronoi diagram

### 6. Aggregation II: Polygons to Polygons
* Intersection and union are still available (`raster`)
* When aggregating different polygon layers, you need to prorate the value of each polygon based on the proportion of the area.
