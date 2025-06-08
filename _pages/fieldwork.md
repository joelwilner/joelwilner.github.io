---
permalink: /fieldwork/
title: "Fieldwork"
layout: single
classes: wide
---

<style>
/* Grid Layout */
.fieldwork-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 1.5rem;
  padding-bottom: 2rem;
}

.fieldwork-card {
  background: #fff;
  border-radius: 10px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
  overflow: hidden;
  cursor: pointer;
  transition: transform 0.2s ease;
}
.fieldwork-card:hover {
  transform: scale(1.02);
}

.fieldwork-card img {
  width: 100%;
  height: 120px;
  object-fit: cover;
}

.fieldwork-content {
  padding: 0.75rem;
}

.fieldwork-content h3 {
  font-size: 1rem;
  margin: 0 0 0.5rem 0;
}

/* Modal Overlay */
.modal-overlay {
  display: none;
  position: fixed;
  top: 0; left: 0;
  width: 100%; height: 100%;
  background: rgba(0,0,0,0.7);
  justify-content: center;
  align-items: center;
  z-index: 1000;
}

.modal-content {
  background: white;
  border-radius: 12px;
  max-width: 700px;
  width: 90%;
  max-height: 90%;
  overflow-y: auto;
  padding: 1.5rem;
  position: relative;
}

.modal-content img {
  width: 100%;
  max-height: 300px;
  object-fit: cover;
  border-radius: 8px;
  margin-bottom: 1rem;
}

.modal-content h2 {
  margin-top: 0;
}

.modal-close {
  position: absolute;
  top: 0.5rem;
  right: 0.75rem;
  background: none;
  border: none;
  font-size: 1.5rem;
  color: #999;
  cursor: pointer;
}
</style>

<!-- Grid of Cards -->
<div class="fieldwork-grid">

<div class="fieldwork-card" onclick="openModal('Site A', 'Longer description of Site A fieldwork, including objectives, data collection methods, and outcomes.', '/assets/images/field1.jpg')">
  <img src="/assets/images/field1.jpg" alt="Fieldwork 1">
  <div class="fieldwork-content">
    <h3>Site A: Coastal Survey</h3>
    <p>Brief: shoreline erosion monitoring.</p>
  </div>
</div>

<div class="fieldwork-card" onclick="openModal('Site B', 'Alpine ecosystem tracking via multispectral drone flights and temperature loggers.', '/assets/images/field2.jpg')">
  <img src="/assets/images/field2.jpg" alt="Fieldwork 2">
  <div class="fieldwork-content">
    <h3>Site B: Alpine Vegetation</h3>
    <p>Brief: mountain ecology study.</p>
  </div>
</div>

<div class="fieldwork-card" onclick="openModal('Site C', 'Urban heat island profiling using remote sensors and community mapping.', '/assets/images/field3.jpg')">
  <img src="/assets/images/field3.jpg" alt="Fieldwork 3">
  <div class="fieldwork-content">
    <h3>Site C: Urban Heat</h3>
    <p>Brief: city climate data collection.</p>
  </div>
</div>

<div class="fieldwork-card" onclick="openModal('Site C', 'Urban heat island profiling using remote sensors and community mapping.', '/assets/images/field3.jpg')">
  <img src="/assets/images/field3.jpg" alt="Fieldwork 3">
  <div class="fieldwork-content">
    <h3>Site C: Urban Heat</h3>
    <p>Brief: city climate data collection.</p>
  </div>
</div>

<div class="fieldwork-card" onclick="openModal('Site C', 'Urban heat island profiling using remote sensors and community mapping.', '/assets/images/field3.jpg')">
  <img src="/assets/images/field3.jpg" alt="Fieldwork 3">
  <div class="fieldwork-content">
    <h3>Site C: Urban Heat</h3>
    <p>Brief: city climate data collection.</p>
  </div>
</div>

<div class="fieldwork-card" onclick="openModal('Site C', 'Urban heat island profiling using remote sensors and community mapping.', '/assets/images/field3.jpg')">
  <img src="/assets/images/field3.jpg" alt="Fieldwork 3">
  <div class="fieldwork-content">
    <h3>Site C: Urban Heat</h3>
    <p>Brief: city climate data collection.</p>
  </div>
</div>
<!-- Add more cards as needed -->

</div>

<!-- Modal Overlay -->
<div class="modal-overlay" id="modalOverlay">
  <div class="modal-content" id="modalContent">
    <button class="modal-close" onclick="closeModal()">×</button>
    <img id="modalImg" src="" alt="">
    <h2 id="modalTitle"></h2>
    <p id="modalDesc"></p>
  </div>
</div>

<script>
function openModal(title, desc, imgSrc) {
  document.getElementById('modalTitle').innerText = title;
  document.getElementById('modalDesc').innerText = desc;
  document.getElementById('modalImg').src = imgSrc;
  document.getElementById('modalOverlay').style.display = 'flex';
}
function closeModal() {
  document.getElementById('modalOverlay').style.display = 'none';
}
</script>

