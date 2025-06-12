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

<!-- Video Container -->
<div class="video-container" style="position: relative; width: 100%; max-width: 600px; margin: auto; margin-bottom: 2rem;">
  <video id="russellVideo" poster="/assets/images/RussellStill.jpg" loop style="width: 100%; border-radius: 8px;">
    <source src="/assets/videos/RussellWebsite.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>

  <!-- Overlay with Play Button and Warning -->
  <div id="videoOverlay" style="position: absolute; top:0; left:0; width:100%; height:100%; 
       background: rgba(0,0,0,0.4); border-radius: 8px; display: flex; flex-direction: column; 
       justify-content: center; align-items: center; cursor: pointer;">
    
    <button id="playButton" style="background: rgba(255,255,255,0.9); border:none; border-radius: 50%; 
            font-size: 2.5rem; width: 64px; height: 64px; line-height: 1; cursor: pointer;">▶</button>
    
    <span id="warningText" style="color: red; font-size: 0.9rem; margin-top: 0.5rem; display: none; text-align: center; max-width: 200px;">
      Photosensitivity warning: flashing images
    </span>
  </div>
</div>

<script>
  const playButton = document.getElementById('playButton');
  const video = document.getElementById('russellVideo');
  const overlay = document.getElementById('videoOverlay');
  const warning = document.getElementById('warningText');

  let hasAcknowledgedWarning = false;

  // Show warning only on hover on desktop (width > 768)
  playButton.addEventListener('mouseenter', () => {
    if(window.innerWidth > 768 && !hasAcknowledgedWarning) {
      warning.style.display = 'block';
    }
  });

  playButton.addEventListener('mouseleave', () => {
    if(window.innerWidth > 768 && !hasAcknowledgedWarning) {
      warning.style.display = 'none';
    }
  });

  // On click, show warning first if not acknowledged, else play video and hide overlay
  playButton.addEventListener('click', () => {
    if (!hasAcknowledgedWarning) {
      warning.style.display = 'block';
      hasAcknowledgedWarning = true;
    } else {
      overlay.style.display = 'none';
      video.play();
    }
  });

  // On mobile, show warning by default
  function checkMobileWarning() {
    if(window.innerWidth <= 768) {
      warning.style.display = 'block';
    } else if (!hasAcknowledgedWarning) {
      warning.style.display = 'none';
    }
  }

  window.addEventListener('resize', checkMobileWarning);
  window.addEventListener('load', checkMobileWarning);
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

