---
title: "What is the geographic identifier?"
sub-title: "This page would include general spreadsheet formatting tips. Examples of badly-structured--> well-structured. Also include info about what geographic identifiers are. Resource to link to: https://www.census.gov/programs-surveys/geography/guidance/geo-identifiers.html"
next-steps:
  - label: "It's an address or cross-street."
    type: resource
    ref: geocoding
  - label: "It's an named place or administrative unit (census geographies, zip codes, school districts, National Parks, etc.)"
    type: resource
    ref: admin-unit
  - label: "It's in latitude and longitude (XY coordinates)."
    type: resource
    ref: lat-long
    
---
# what-is-geo-id

Many times you might have data that has geographic information in a table form. Geographic information might include: an address or cross-street, an administrative unit (e.g. census geographies, zip codes, provinces, territories, school districts, etc.), XY coordinates (e.g. latitude and longitude), or place names. Sometimes the geographic identifier is easily understandable such as a county name. Other times a unique identifier such as a FIPS code will be the geographic identifier that can be used. 

It just takes a little work to convert your geographic information into a geospatial format. 

You might choose different approaches depending on how you wish to visualize your data on your map. Some methods result in points while others represent results in areas. 

## Addresses

Addresses may be in a single field or in multiple fields. They may be street blocks, or missing the actual street number. P.O. Boxes will only map to the Zip code, not the actual address. Addresses are typically visualized as points.

Some examples:

* 124 Main Street  
* 2400 Block of Elm St  
* 917 1st Avenue, Anywhere, CA, 12398

## Administrative units 

(census geographies, zip codes, school districts, etc.)  
Administrative units may vary greatly based on your area of interest. Administrative units also vary around the world. Administrative units are typically visualized as areas (polygons). 

Some examples:

* Census block/tract/group  \-   
* Zip codes (5 or 9 digit) \- 12398 or 12398-3485  
* State name \- California or 06 (FIPS code)  
* Voting district \- San Francisco Supervisorial District 1  
* Parcel numbers

## Place names & points of interest

Place names can be interesting. The approach you select will depend on how you want to visualize the data. They may also require some data wrangling. Place names and points of interest can be represented by points or areas (polygons) depending on the method that you use. 

* FIPS  
* GNIS

## XY coordinates (latitude and longitude)

With XY coordinates, the X value indicates how far east or west a feature is (longitude), and the Y value indicates how far north or south it is (latitude). Negative values are possible. XY coordinates can come in a number of formats. These are visualized as points.

* 37.375184, \-120.419319  
* 37° 22' 30.6624", \- 120° 25' 9.5484"  
* 37° 22.51104', \- 120° 25.15914'  
* Easting: 487,000 m, Northing: 3,618,000 m



