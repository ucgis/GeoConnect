---
layout: home
title: UC GIS Consultation Tool
---

<div class="home-page">

  <div class="hero">
    <h1>GIS Interactive Guide</h1>
    <p class="hero-subtitle">
      Your guided walk-through to help you with finding, cleaning, choosing a platform,
      and visualizing data to map with GIS. Created by the University of California (UC)
      GIS Librarians to help you with your geospatial research needs.
    </p>
  </div>

  <div class="home-content">
    <p>Choose a starting point below, or begin with the most common question:</p>
  </div>

  <div class="starting-points">
    <h2>Common Starting Points</h2>

    <div class="cards-grid">

{% assign q1 = site.questions | where: "slug", "what-do-you-want-to-map" | first %}
{% if q1 %}
<div class="card card-featured">
  1.url | relative_url }}" class="card-link">
    ```html <div class= }}" class="card-link"> <div class="card-content"> <h3>{{ q1.title }}</h3> {% if q1.sub-title %} <p class="card-subtitle">{{ q1.sub-title }}</p> {% endif %} </div> <div class="card-arrow">→</div> </a> </div> {% endif %}
{% assign q2 = site.questions | where: "slug", "finding-gis-data" | first %}
{% if q2 %}
```html<div class="card card-featured">
  2.url | relative_url }}" class="card-link">
    <div class="card-content">
      <h3>{{ q2.title }}</h3>
      {% if q2.sub-title %}
      <p class="card-subtitle">{{ q2.sub-title }}</p>
      {% endif %}
    </div>
    <div class="card-arrow">→</div>
  </a>
</div>
{% endif %}
{% assign q3 = site.questions | where: "slug", "choose-a-platform" | first %}
{% if q3 %}
<div class="card card-featured">
  3.url | relative_url }}" class="card-link">
    <div class="card-content">
      <h3>{{ q3.title }}</h3>
      {% if q3.sub-title %}
      <p class="card-subtitle">{{ q3.sub-title }}</p>
      {% endif %}
    </div>
    <div class="card-arrow">→</div>
  </a>
</div>
{% endif %}
  <div class="about-section">
    <h2>About This Tool</h2>

    <p>
      Thank you for visiting. Our website is currently under development as we continue
      to build and refine content to better serve our community. This initial version
      provides a foundation for the information and resources we plan to offer.
      Additional sections, features, and content will be added over time based on user
      feedback and evolving needs.
    </p>

    <p>
      We appreciate your patience and welcome your suggestions as we work to create a
      more comprehensive and useful experience.
    </p>

    <p>
      UC GIS Librarians have extensive knowledge and frequently conduct consultations
      with predictable pathways and decision points. This tool guides you through those
      same decisions to help you find the resources and guidance you need.
    </p>

    <p>
      <strong>Need direct help?</strong>
      <a href="https://docs.google.com/spreadsheets/d/1xkgsnwz5MXEIpD9OMWajIPKpSdTdlb7THoeWCirHR7A/edit?usp=sharing"
        target="_blank"
        rel="noopener noreferrer">
        Contact a UC GIS librarian
      </a>
      for a personal consultation.
    </p>

  </div>

</div>
