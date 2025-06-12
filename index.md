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

.teaser {
  position: relative;
  height: 200px;
  overflow: hidden;
}

.teaser video,
.teaser img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.video-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0,0,0,0.4);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  color: white;
  cursor: pointer;
  transition: background 0.3s;
}

.video-overlay:hover {
  background: rgba(0,0,0,0.6);
}

.video-overlay span.warning {
  font-size: 0.75rem;
  margin-top: 0.5rem;
  opacity: 0;
  transition: opacity 0.3s;
}

.video-overlay:hover span.warning {
  opacity: 1;
}

.video-overlay .play-button {
  font-size: 2rem;
  background: rgba(255,255,255,0.2);
  padding: 0.5rem 1rem;
  border-radius: 8px;
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
      <video id="russellVideo" poster="/assets/images/Ross.jpg">
        <source src="/assets/videos/RussellWebsite.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <div class="video-overlay" onclick="playVideo()">
        <div class="play-button">▶ Play</div>
        <span class="warning">Photosensitivity warning: flashing images</span>
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
function playVideo() {
  const video = document.getElementById('russellVideo');
  const overlay = video.nextElementSibling;
  overlay.style.display = 'none';
  video.play();
}
</script>

