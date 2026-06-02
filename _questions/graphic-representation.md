---
title: "Let's check that the data coverage is what you need."
sub-title: "Do you just want to map locations, or are you trying to map something about the data?"
parent: "previous page"
permalink: "test-test"
next-steps:
  - label: ""I'm just mapping locations.""
    type: question
    ref: finalize-map
  - label: ""I'd like to map something about the data.""
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

Optional description content here.

<!-- Expand / Collapse Controls -->
<div style="margin: 1.5rem 0;">
  <button onclick="expandAll()">Expand all</button>
  <button onclick="collapseAll()">Collapse all</button>
</div>
<details class="collapsible">
<summary><strong>title</strong></summary>

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
