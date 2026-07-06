---
title: "Here's some information about how to work with images."
sub-title: "Brief description"
jobs_to_be_done:
  - "Goal 1"
  - "Goal 2"
steps:
  - "Step 1 instructions"
  - "Step 2 instructions"
next-steps:
    - label: "Yes, it's a digitized image of a map"  
    type: question  
    ref: do-you-have-data  
   - label: "I'd like to map something about the data."  
    type: resource  
    ref: qual-quant   
---
<nav class="breadcrumbs">
  <a href="{{ '/' | relative_url }}">do-you-have-data</a>

  {% if page.parent %}
    /
    <a href="{{ page.parent_url | relative_url }}">{{ page.parent }}</a>
  {% endif %}

  /
  <span>{{ page.title }}</span>
</nav>
Working with images in GIS can involve integrating spatial photos or historical maps/data with geographic data to map, measure and analyze new information or changes over time. Sometimes having the image displayed in the GIS is all that’s needed; in other cases, you may want to extract features from the scanned image by creating a point, line, or polygon layer in the GIS.

**Georeferencing your images**

If you upload a scanned image of a map to a GIS, the platform doesn’t initially recognize where the map is located and how it fits on the basemap. The process of assigning geographic coordinates (latitude and longitude) to digital imagery, such as scanned historical maps, is called georeferencing. GIS platforms have georeferencing tools that enable you to align the scanned map properly on the basemap. This involves shifting, scaling, and rotating images:

1. Identify control points: select recognizable features on your image, such as road intersections, coastlines, and building corners.   
2. Link to control points or known coordinates: match points to the exact same locations on a pre-existing, spatially referenced basemap.   
3. Evaluate the accuracy using the Root Mean Square Error (RMSE) and adjust control points if necessary.  
4. Export or save: once aligned, the spatial data can be saved as a GeoTIFF or GeoPDF, allowing GIS software to place the image where it belongs on the globe. 

Example: Suppose you have a scanned historical map:
<!-- Expand / Collapse Controls -->
<div style="margin: 1.5rem 0;">
  <button onclick="expandAll()">Expand all</button>
  <button onclick="collapseAll()">Collapse all</button>
</div>
<details class="collapsible">
1. On the scanned map, identify a road intersection.  
2. Find that exact intersection on a georeferenced aerial image or basemap.  
3. Repeat for several well-distributed locations.  
4. The GIS software uses these matched control points to calculate the transformation and place the map in its correct geographic position.
</details>

<script>
function expandAll() {
  document.querySelectorAll('details.collapsible')
    .forEach(d => d.open = true);
}

function collapseAll() {
  document.querySelectorAll('details.collapsible')
    .forEach(d => d.open = false);
}
</script>

Some platforms, such as ArcGIS Online and Google Earth Pro, allow the user to match a scanned image to the basemap by dragging and rotating it, then pinning identifiable locations on the image to the same location on the basemap. (In ArcGIS Online, the relevant tool is called Add Media Layer.) This is sometimes referred to as rubber-sheeting. This approach may be useful when a high level of precision is not required.

* *Is your image already georeferenced?*   
  * *When you open the data in a GIS program, does it have a coordinate system? One way to find out is if the data has a .prj or a world file (.tfw, .jfw). If your image has a (0,0) coordinate*   
  * *Do you have an image downloaded from a public website (USGS, USDA, NASA)?*   
    * *Such websites are more likely to provide georeferenced images.*  
  * *Are these historic images or contemporary?*  
    * *Contemporary images are more likely to have locational information in the file.*   
  * *A file designated as a GeoTIFF is already georeferenced.*  
* *Did you download the data from an authoritative source (David Rumsey), or did you scan the image yourself?*   
  * *The quality of the scan may influence how easily the image can be georeferenced.*


  
**Common Use Cases**

* Historical mapping: lay old paper maps or city plans over modern satellite imagery.   
  * **Note** \- Historic Maps that are hand drawn will have errors and it may be difficult to match the map to real world coordinates. The process of georeferencing the image may be iterative and distort some areas while preserving others.   
* Urban planning: align unreferenced architectural or engineering drawings to evaluate properly lines or utility layouts.  
* Environmental analysis: overlay drone or satellite imagery over topographic data to map flood zones, wildlife habitats or deforestation. 

**Resources:**  
	**Georeferencing**

* Imagery and Its Use in GIS: [https://www.geographyrealm.com/imagery-use-gis/](https://www.geographyrealm.com/imagery-use-gis/)  
* Georeference historical imagery in ArcGIS Pro:  
* [https://learn.arcgis.com/en/projects/georeference-imagery-in-arcgis-pro/](https://learn.arcgis.com/en/projects/georeference-imagery-in-arcgis-pro/)  
* Georeferencing a Map (QGIS):  [https://docs.qgis.org/3.44/en/docs/training\_manual/forestry/map\_georeferencing.html](https://docs.qgis.org/3.44/en/docs/training_manual/forestry/map_georeferencing.html)  
* Hand-drawn historic maps: Utilization and conversion of unique features into Geographic Information Systems: [https://www.tandfonline.com/doi/full/10.1080/15420353.2024.2399714\#abstract](https://www.tandfonline.com/doi/full/10.1080/15420353.2024.2399714#abstract)

**Creating points / lines /polygons**

* Creating lines and polygons: [https://training.caltopo.com/all\_users/objects/lines-and-polys](https://training.caltopo.com/all_users/objects/lines-and-polys)  
* Create a Layer and Add Features in ArcGIS Online:			

  https://www.esri.com/about/newsroom/arcwatch/create-a-layer-and-add-features-in-arcgis-online

* Create points on a map (ArcGIS Pro): [https://doc.esri.com/en/arcgis-pro/latest/get-started/create-points-on-a-map.html](https://doc.esri.com/en/arcgis-pro/latest/get-started/create-points-on-a-map.html)  
* Create features in QGIS: [https://docs.qgis.org/3.44/en/docs/training\_manual/create\_vector\_data/create\_new\_vector.html](https://docs.qgis.org/3.44/en/docs/training_manual/create_vector_data/create_new_vector.html) 

