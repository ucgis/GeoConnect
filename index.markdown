---
layout: home
title: GeoNavigator
---

<div class="home-page">

  <div class="hero">
    <h1>GeoNavigator</h1>
    <p class="hero-subtitle">
A choose-your-own adventure for creating maps and working with GIS data. This guided walk-through will support you with finding, cleaning, and visualizing data to create maps, as well as selecting the best platform.</p>
<p>Created by librarians and GIS staff across multiple University of California (UC) campuses to centralize support for beginning and intermediate mappers with geospatial research and map creation.</p>
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
  <a href="{{ q1.url | relative_url }}" class="card-content">
      <h3>{{ q1.title }}</h3>
      {% if q1.sub-title %}
      <p class="card-subtitle">{{ q1.sub-title }}</p>
      {% endif %}
    <div class="card-arrow">→</div>
  </a>
</div>
{% endif %}

{% assign q2 = site.resources | where: "slug", "finding-gis-data" | first %}
{% if q2 %}
<div class="card card-featured">
  <a href="{{ q2.url | relative_url }}" class="card-content">
      <h3>{{ q2.title }}</h3>
      {% if q2.sub-title %}
      <p class="card-subtitle">{{ q2.sub-title }}</p>
      {% endif %}
    <div class="card-arrow">→</div>
  </a>
</div>
{% endif %}

{% assign q3 = site.questions | where: "slug", "choose-a-platform" | first %}
{% if q3 %}
<div class="card card-featured">
  <a href="{{ q3.url | relative_url }}" class="card-content">
      <h3>{{ q3.title }}</h3>
      {% if q3.sub-title %}
      <p class="card-subtitle">{{ q3.sub-title }}</p>
      {% endif %}
    <div class="card-arrow">→</div>
  </a>
</div>
{% endif %}

</div>
  <div class="about-section">
    <h2>About This Tool</h2>
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
    <p>
      Thank you for visiting. Our website is currently under development as we continue
      to build and refine content to better serve our community. This initial version
      provides a foundation for the information and resources we plan to offer.
      Additional sections, features, and content will be added over time based on user
      feedback and evolving needs.
    </p>

    <p>
      We appreciate your patience and [welcome your suggestions](https://forms.gle/Kt7dicLdwbsta6aX6) as we work to create a
      more comprehensive and useful experience.
      </p>
</div>
