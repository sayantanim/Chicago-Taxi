# Chicago-Taxi


Data Analysis and Visualization of Chicago Taxi Data

Data analysis and visualization performed for the year 2016. 

Pandas and Geopandas used for this exercise.

### Change Log:
**Date: Feb 20, 2017**
* Taxi Trips for Chicago on Open Data Portal was updated on 02/10/2017. This now contains complete 2016 data. When last updated on 01/19/2017, it contained data till 10/01/2016.
* Hence 2016 can now be visualized completely.
* Intitally, I had dropped all null values which resulted in a good amount of data loss owing to the fact that a large number of trips don't have Pickup and Dropoff Census Tracts. Thus, now I dropped the Pickup and Dropoff Census Tracts column first and then used `df.dropna()` to filter the null values.
* I also added another column 'Date' which was used to figure find the variation of rides per day over the year.
* 'Community Areas' column is no longer a part of the dataset uploaded on the portal.
* I also removed the dpi value in the scatter plot showing the 'Pickup Centroid Locations'. In this graph, the grid is off as well.
* Hence I used `grid=True` in the next plot so that the grids are visible.
* I added 2 more plots both for showing 'Trip Miles' vs. 'Trip Total'.
* Also changed `set_axis_bgcolor` to `set_facecolor` as per the following warning:
  * MatplotlibDeprecationWarning: The set_axis_bgcolor function was deprecated in version 2.0. Use set_facecolor instead.
