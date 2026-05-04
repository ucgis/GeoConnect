---
title: "Do you have the data you need?"
sub-title: "Here are some questions to think through about your data before you get started mapping. List of data assessment questions."
permalink: /data-you-need/
---

To get started mapping, you’ll need data that’s tied to locations. Knowing what format your data is in will help you map it in the most efficient way.

<!-- Expand / Collapse Controls -->
<div style="margin: 1.5rem 0;">
  <button onclick="expandAll()">Expand all</button>
  <button onclick="collapseAll()">Collapse all</button>
</div>

<details class="collapsible">
<summary><strong>GIS Files + Online Platforms</strong></summary>

- Shapefile  
- GeoJSON  
- KML/KMZ  
- GeoTIFF  

</details>

<details class="collapsible">
<summary><strong>Spreadsheets</strong></summary>

- CSV  
- XLSX  
- TXT  

</details>

<details class="collapsible">
<summary><strong>Image</strong></summary>

Scanned maps can be used in GIS platforms.

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



