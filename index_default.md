---
layout: splash
title: "Joel Wilner"
header:
  overlay_image: /assets/images/websitebanner.jpg
  overlay_filter: "0.3"
  caption: ""
excerpt: "Decoding glacial and erosive systems in a warming world."
intro:
  - excerpt: 'Welcome to my personal site. I’m a glaciologist, glacial geologist, and adventurer.'
---

<style>
.feature-row-custom {
  display: flex;
  gap: 1.5rem;
  flex-wrap: wrap;
  justify-content: center;
  margin-top: 2rem;
}

.feature-card {
  flex: 1 1 300px;
  max-width: 340px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  border-radius: 8px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
  overflow: hidden;
  background: white;
}

.feature-card .teaser {
  height: 200px;
  overflow: hidden;
}

.feature-card img,
.feature-card video {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.feature-card .content {
  padding: 1rem;
  flex-grow: 1;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.feature-card h2 {
  font-size: 1.25rem;
  margin: 0 0 0.5rem 0;
}

.feature-card a {
  margin-top: 1rem;
}
</style>

<div class="feature-row-custom">

  <!-- Video Card -->
  <div class="feature-card">
    <div class="teaser">
      <video autoplay muted loop playsinline>
        <source src="/assets/videos/RussellWebsite.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
    </div>
    <div class="content">
      <h2>Calving dynamics</h2>
      <a href="/aboutme/" class="btn btn--primary">Read More</a>
    </div>
  </div>

  <!-- Image Card 1 -->
  <div class="feature-card">
    <div class="teaser">
      <img src="/assets/images/RussellErosion.jpg" alt="Glacial erosion">
    </div>
    <div class="content">
      <h2>Glacial erosion</h2>
      <a href="/research/" class="btn btn--primary">Read More</a>
    </div>
  </div>

  <!-- Image Card 2 -->
  <div class="feature-card">
    <div class="teaser">
      <img src="/assets/images/Frontino.png" alt="Tropical paleoclimate">
    </div>
    <div class="content">
      <h2>Tropical paleoclimate</h2>
      <a href="/peakbagging/" class="btn btn--primary">Read More</a>
    </div>
  </div>

</div>

