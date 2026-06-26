---
layout: home
title: UC GIS Consultation Tool
---
{% include proof_banner.html %}
<div class="home-page">
  <div class="hero">
    <h1>GIS Research Consultation Guide</h1>
    <p class="hero-subtitle">Interactive guidance from UC GIS Librarians to help you with your geospatial research needs.</p>
  </div>

  <div class="home-content">
    <p>Choose a starting point below, or begin with the most common question:</p>
  </div>

  <div class="starting-points">
    <h2>Common Starting Points</h2>
    <div class="cards-grid">
      {% assign start_question = site.questions | where: "slug", "do-you-have-data" | first %}
      {% if start_question %}
      <div class="card card-featured card-question">
        <a href="{{ start_question.url | relative_url }}" class="card-link">
          <div class="card-icon">
            <i data-lucide="git-branch"></i>
          </div>
          <div class="card-content">
            <h3>{{ start_question.title }}</h3>
            {% if start_question.sub-title %}
            <p class="card-subtitle">{{ start_question.sub-title }}</p>
            {% endif %}
          </div>
          <div class="card-arrow">→</div>
        </a>
      </div>
      {% endif %}

{% assign start_question = site.questions | where: "slug", "graphic-representation" | first %}
      {% if start_question %}
      <div class="card card-featured card-question">
        <a href="{{ start_question.url | relative_url }}" class="card-link">
          <div class="card-icon">
            <i data-lucide="map"></i>
          </div>
          <div class="card-content">
            <h3>Is the data coverage what you need?</h3>
            <p class="card-subtitle coming-soon">Does it cover the area, scale, time frame, or is it not detailed enough?</p>
          </div>
        </div>
      </div>
      
<!-- Placeholder cards for future starting points -->
      <div class="card card-question">
        <div class="card-link card-disabled">
          <div class="card-icon">
            <i data-lucide="sparkles"></i>
          </div>
          <div class="card-content">
            <h3>I need to analyze spatial patterns</h3>
            <p class="card-subtitle coming-soon">Coming soon!</p>
          </div>
        </div>
      </div>

      <div class="card card-resource">
        <div class="card-link card-disabled">
          <div class="card-icon">
            <i data-lucide="globe"></i>
          </div>
          <div class="card-content">
            <h3>I need to create a web map</h3>
            <p class="card-subtitle coming-soon">Coming soon!</p>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div class="about-section">
    <h2>About This Tool</h2>
    <p>UC GIS Librarians have extensive knowledge and frequently conduct consultations with predictable pathways and decision points. This tool guides you through those same decisions to help you find the resources and guidance you need.</p>
    <p><strong>Need direct help?</strong> <a href="https://docs.google.com/spreadsheets/d/1xkgsnwz5MXEIpD9OMWajIPKpSdTdlb7THoeWCirHR7A/edit?usp=sharing">Contact a UC GIS librarian</a> for a personal consultation.</p>
  </div>
</div>
