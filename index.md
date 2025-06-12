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
  position: relative;
  overflow: hidden;
}

.feature-card img,
.feature-card video {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

#videoOverlay {
  position: absolute;
  top: 0; left: 0;
  width: 100%; height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  transition: background-color 0.3s ease;
  pointer-events: none; /* prevent hover issues */
}

.teaser:hover #videoOverlay {
  background-color: rgba(0, 0, 0, 0.4);
}

#playButton {
  background: rgba(255, 255, 255, 0.9);
  border: none;
  border-radius: 50%;
  font-size: 2.5rem;
  width: 64px;
  height: 64px;
  cursor: pointer;
  color: black;
  box-shadow: 0 0 6px rgba(0,0,0,0.3);
  z-index: 10;
  pointer-events: all;
  position: relative;
}

#warningText {
  color: white;
  font-size: 0.85rem;
  margin-top: 0.5rem;
  max-width: 220px;
  text-align: center;
  user-select: none;
  pointer-events: none;
  display: none;
}

/* Desktop: show warning only on hover/focus */
@media (min-width: 769px) {
  #playButton:hover + #warningText,
  #playButton:focus + #warningText {
    display: block;
  }
}

/* Mobile: always show warning */
@media (max-width: 768px) {
  #warningText {
    display: block !important;
  }
}
</style>

<div class="feature-row-custom">

  <!-- Video Card -->
  <div class="feature-card">
    <div class="teaser">
      <video id="russellVideo" poster="/assets/images/RussellStill.jpg" loop muted playsinline>
        <source src="/assets/videos/RussellWebsite.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>

      <div id="videoOverlay">
        <button id="playButton" aria-label="Play Video" title="Play video">▶</button>
        <span id="warningText">Photosensitivity warning: flashing images</span>
      </div>
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

<script>
  const playButton = document.getElementById('playButton');
  const video = document.getElementById('russellVideo');
  const overlay = document.getElementById('videoOverlay');

  playButton.addEventListener('click', () => {
    overlay.style.display = 'none';
    video.play();
  });
</script>

