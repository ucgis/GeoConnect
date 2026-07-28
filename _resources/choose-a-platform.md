---
title: "Let's choose a platform for your map."
sub-title: "Brief description"
jobs_to_be_done:
  - "Goal 1"
  - "Goal 2"
steps:
  - "Step 1 instructions"
  - "Step 2 instructions"
next-steps:
  - label: "I'm ready to get started mapping! I know which platform I want to use."
    type: question
    ref: related-question
---
<nav class="breadcrumbs">
  <a href="{{ '/' | relative_url }}">Home</a>

  {% if page.parent %}
    /
    <a href="{{ page.parent_url | relative_url }}">{{ page.parent }}</a>
  {% endif %}

  /
  <span>{{ page.title }}</span>
</nav>
Choosing an appropriate GIS platform for your needs comes down to your goals, timeframe, and GIS expertise. Do you need to make simple web maps, do complex spatial analysis, or manage large sets of data?  

Not all GIS or mapping platforms are the same\! While almost all of them can perform basic mapping tasks, some are complicated to learn because they can perform specialized or computational tasks in addition to the basics. Other platforms are focused on telling stories with maps. Some are web-based, others need to be installed on your device. While some platforms are well-known, more obscure ones may be exactly what you need.

Everyone’s needs for making a map can vary widely. Here is some guidance that can help frame your choice of an appropriate platform.

* *What do you need to do?*   
  * *If you just need to plot locations, create a heat map, or tell a visual story, you don't need something with heavy analytical software.*  
  * *If you plan to do data manipulation, raster/vector geoprocessing, 3D mapping, etc., then choose a product that provides more robust analytics.*  
* *Do you have experience working with GIS software previously? Do you have a deadline?*  
  * *If you don't have much experience or are on a tight deadline, choose a simpler platform that might feature drag and drop functionality and requires little to no training to use. If you have the time and are already familiar with GIS tools, consider choosing a platform with more features for creating the map you envision.*  
* *What is your computing platform (Windows / Mac)?*  
  * *Esri’s ArcGIS Pro only runs well on Windows machines, although you might have the option of accessing it through a virtual machine. By contrast, QGIS will run equally well on multiple computing platforms.*  
* *What type of files are you working with? (raster / vector) Are you creating data or using existing data?*   
  * *GIS platforms vary in their ability to work with different data formats, including data you collected (drone, GPS, etc.) or data from external sources.*  
  * *If you want to analyze raster data, talk to your librarian about specialized tool options.*  
* *Are you working alone or with a group?*  
  * *Platforms such as ArcGIS Online allow for collaboration in groups, and for crowd-sourced updates to a map. Some desktop GIS provide the means for collaborative work. Usually, only one person can work on the map at a time.*  
* *Do you have a preference between vendor based systems vs. open source platforms?*   
  * *Vendor based (subscription required): users can access this software by individual subscription or through a campus subscription. Such platforms tend to come with support, extensive documentation, and possibly integration with other tools. Some vendor tools have freemium business models, where you can use a basic version for free but would have to pay for advanced capabilities.*  
  * *Open Source (no subscription required): free to use and community driven. Tends to have community support. A benefit of using open source software is that you will maintain access when you leave the university.*   
* *Do you need to share your work through an interactive platform (maps, tables, narrative)?*   
  * *Some platforms are designed for easily sharing maps and visualizations online.*  
* *Are you sharing work and data with non GIS users?*   
  * *Consider a platform that provides an easy-to-understand user interface.*  
* *Do you need to keep a level of security around your data?*  
  * *ArcGIS Online allows different levels of sharing. Choose a desktop platform if you need to restrict access to elements of your data.*  
  * *Check with your librarian to get more guidance if data security is a concern.*

Don’t know where to begin in choosing a GIS platform? Take a look at the [GIS and Digital Mapping Tools matrix](https://docs.google.com/spreadsheets/d/e/2PACX-1vRO90zVdeOgK7gMNa1lLuP7RfZXsqB0SYuW5vgmRsOMpWjlg9ruUbjiSSIf8lqq5OiCp0f6tLDTHOEr/pubhtml) compiled by UC Riverside Library. The matrix evaluates the capabilities of several mapping platforms side by side all in one view, with additional tabs that only show tools related to making a map, analyzing spatial data, or creating a narrative with maps. The [associated library research guide](https://guides.lib.ucr.edu/c.php?g=171041&p=8392166) contains additional information about each tool.

