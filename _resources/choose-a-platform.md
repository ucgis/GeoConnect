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
  - label: "Next action"
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

Additional detailed content in markdown format.
