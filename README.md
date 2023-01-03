## Abstract
Libraries are recognized as an important part of a city. In addition to the educational resources they provide, libraries generate social capital. This study investigates if the city of Minneapolis, MN provides equitable access to libraries based on distance from a library and the racial makeup of each census block. Distance is measured as a straight line from centroids of each census block to the nearest library. Using Minneapolis’s 5964 census blocks, we find no signs of discrimination based upon not being white. Libraries tend to be located closer to areas with more people of color and higher population density.

## Associated Papers
Regression Analysis <br/>
Economic Inequality

## Methodology
As a case study of library accessibility, I decided to study the distribution of public libraries in Minneapolis in comparison with racial demographics throughout the city. Population data was taken from the 2020 US census at the block level – the smallest division publicly available with 5964 blocks in the city of Minneapolis. People were categorized as either white or not white where multi racial individuals were part of the non-white group. All data cleaning and linear regression was done in R. The population data was plotted and analyzed with the library locations in ArcGIS using central place theory. Central place theory is the assumption that a customer will patronize the closest central place. This analysis used a straight-line approach which does not account for landmark barriers (rivers, lakes, highways, etc). A more nuanced approach would calculate the travel distance by road. Since this study is about inequality, access via public transit or walking could also be considered in future analysis.

## Data Sources
- The list of libraries in the Twin cities came from the [MN DEPARTMENT OF EDUCATION](https://education.mn.gov/MDE/dse/Lib/sls/stat/)<br/>
- They were geocoded using the [US Census Geocoder](https://geocoding.geo.census.gov/geocoder/) you can find the user guide [here](https://www2.census.gov/geo/pdfs/maps-data/data/Census_Geocoder_User_Guide.pdf) (page 18). Shapefiles can be downloaded [here](https://www.census.gov/cgi-bin/geo/shapefiles/index.php)
- Racial data was compiled at the block level from the 2020 decenial census
