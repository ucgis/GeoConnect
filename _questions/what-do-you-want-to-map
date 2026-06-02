---
title: "what-do-you-want-to-map"
sub-title: "What map do you want to create?"
parent: "previous page"
permalink: "test-test"

next-steps:
  - label: "I want to map locations"
    type: question
    ref: map-locations
  - label: "Do you want to create a shaded area (thematic) map?"
    type: resource
    ref: map-thematic
  - label: "I want to make something more complicated"
    type: resource
    ref: get-help
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
