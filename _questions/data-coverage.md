---
title: "Let's check that the data coverage is what you need."
sub-title: "Do you just want to map locations, or are you trying to map something about the data?"
parent: "ingest-data"
permalink: /data-coverage/
next-steps:
  - label: "I'm just mapping locations."
    type: question
    ref: finalize-map
  - label: "I'd like to map something about the data."
    type: resource
    ref: qual-quant
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

Before going any further with mapping the data, make sure it completely covers the area you expected it to. If it doesn’t, there may be an issue with the way the data loaded into the GIS, or it may be that the data you acquired has gaps or a smaller extent than what you expected.

* Is your data in the right part of the world?
  * Check and reformat your x,y data if needed. 
  * For geocoded addresses, you may need to do some additional data cleanup
* Does it cover the geographic area you expect your data to cover?
  * Different data providers may have different definitions for the geographic extent of natural features (e.g. the Sonoran Desert) or populated regions (e.g. the greater Los Angeles area). You may have to return to searching for data.
  * In some datasets, sensitive regions such as military installations may be excluded, creating holes in the area covered.
* Is any of the data missing? (Geographic coverage, Is the data outdated? Do you need something more recent?, etc.)
  * Determine which data is missing and conduct a search for new/additional data.
* Is there an issue with the data upload? (Are there missing rows, ex. The table has 200 rows but you only have 50.)
  * Check your original dataset and reupload to see if that resolves the issue.
* Is your data too generalized? 
  * You may need to find a more specific dataset if the data is too general for your area.

This is not an exhaustive list of questions, rather a guide to help you while you search for the data that is best for your project. 
