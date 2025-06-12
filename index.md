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

<!-- Video Embed with Play Button and Photosensitivity Warning -->
<div class="video-container" style="position: relative; width: 100%; max-width: 600px; margin: auto; margin-bottom: 2rem;">
  <video id="russellVideo" poster="/assets/images/RussellStill.jpg" loop style="width: 100%; border-radius: 8px;">
    <source src="/assets/videos/RussellWebsite.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>

  <div class="video-overlay" id="videoOverlay" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; background-color: rgba(0,0,0,0.4); display: flex; flex-direction: column; justify-content: center; align-items: center; border-radius: 8px;">
    <button id="playButton" style="background: rgba(255,255,255,0.8); border: none; border-radius: 50%; padding: 0.75rem 1rem; font-size: 2rem; cursor: pointer;">▶</button>
    <span class="warning" id="warningText" style="display: none; color: red; font-size: 0.9rem; margin-top: 0.5rem;">Photosensitivity warning: flashing images</span>
  </div>
</div>

<!-- JavaScript for Play Button and Warning -->
<script>
  const playButton = document.getElementById('playButton');
  const video = document.getElementById('russellVideo');
  const overlay = document.getElementById('videoOverlay');
  const warning = document.getElementById('warningText');

  let hasAcknowledgedWarning = false;

  playButton.addEventListener('mouseenter', () => {
    warning.style.display = 'block';
  });

  playButton.addEventListener('mouseleave', () => {
    if (!hasAcknowledgedWarning) {
      warning.style.display = 'none';
    }
  });

  playButton.addEventListener('click', () => {
    if (!hasAcknowledgedWarning) {
      warning.style.display = 'block';
      hasAcknowledgedWarning = true;
    } else {
      overlay.style.display = 'none';
      video.play();
    }
  });
</script>

<!-- Feature Section -->
  <div class="feature-card">
    <div class="teaser">
      <img src="/assets/images/RussellErosion.jpg" alt="Glacial erosion">
    </div>
    <div class="content">
      <h2>Glacial erosion</h2>
      <a href="/research/" class="btn btn--primary">Read More</a>
    </div>
  </div>

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
function playVideo() {
  const video = document.getElementById('russellVideo');
  const overlay = document.getElementById('videoOverlay');
  overlay.style.display = 'none';
  video.play();
}
</script>

