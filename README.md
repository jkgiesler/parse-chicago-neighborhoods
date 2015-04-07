# chicago_neighborhoods
Determining Chicago neighborhood from latitude and longitude.

Playing around with data.cityofchicago.org, I quickly found that the community id numbers were all but useless. Most of the data sources had GPS coordinates, but no community id. In order to fix this I wrote this small script to find a neighborhood given GPS coordinates. Neighborhoods can then be mapped easily to community id.

The script uses a GeoJSON file containing polygons of Chicago neighborhoods. Once all of the polygons have been generated, a simple point in polygon algorithm is used to determine which neighborhood contains the point of interest.
