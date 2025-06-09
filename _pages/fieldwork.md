---
permalink: /fieldwork/
title: "Fieldwork"
layout: single
classes: wide
---

<style>
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

/* Detail View */
#fieldworkDetail {
  padding: 1rem;
  background: #fff;
  border-radius: 10px;
  box-shadow: 0 0 8px rgba(0,0,0,0.1);
}

#fieldworkDetail img {
  width: 100%;
  max-height: 300px;
  object-fit: cover;
  margin-bottom: 1rem;
  border-radius: 8px;
}

#fieldworkDetail button {
  margin-bottom: 1rem;
  background: none;
  border: none;
  color: #007acc;
  font-size: 1rem;
  cursor: pointer;
  padding: 0;
}
#fieldworkDetail button:hover {
  text-decoration: underline;
}
</style>

<!-- Grid of Fieldwork Cards -->
<div id="fieldworkGrid" class="fieldwork-grid">

  <div class="fieldwork-card" onclick="showDetail('site-a')">
    <img src="/assets/images/field1.jpg" alt="Site A">
    <div class="fieldwork-content">
      <h3>Site A: Coastal Survey</h3>
      <p>Brief: shoreline erosion monitoring.</p>
    </div>
  </div>

  <div class="fieldwork-card" onclick="showDetail('site-b')">
    <img src="/assets/images/field2.jpg" alt="Site B">
    <div class="fieldwork-content">
      <h3>Site B: Alpine Vegetation</h3>
      <p>Brief: alpine ecosystem monitoring.</p>
    </div>
  </div>

  <div class="fieldwork-card" onclick="showDetail('site-c')">
    <img src="/assets/images/field3.jpg" alt="Site C">
    <div class="fieldwork-content">
      <h3>Site C: Urban Heat</h3>
      <p>Brief: city climate data collection.</p>
    </div>
  </div>

</div>

<!-- Detail View -->
<div id="fieldworkDetail" style="display: none;">
  <button onclick="returnToGrid()">← Back to Fieldwork</button>
  <div id="detailContent"></div>
</div>

<script>
const fieldworkData = {
  'site-a': {
    title: 'Site A: Coastal Survey',
    img: '/assets/images/field1.jpg',
    desc: 'This project monitors shoreline erosion using UAV imagery and in-situ water quality sensors. Long-term data collection contributes to coastal resilience modeling and hazard prediction.'
  },
  'site-b': {
    title: 'Site B: Alpine Vegetation',
    img: '/assets/images/field2.jpg',
    desc: 'At high-elevation sites, vegetation shifts were monitored using NDVI imagery and soil sampling. This project helps understand climate change impacts on alpine ecosystems.'
  },
  'site-c': {
    title: 'Site C: Urban Heat',
    img: '/assets/images/field3.jpg',
    desc: 'Using remote temperature sensors and community surveys, this project mapped urban heat islands in metro areas to inform sustainable planning and public health strategies.'
  }
};

function showDetail(key) {
  const data = fieldworkData[key];
  const container = document.getElementById('detailContent');
  container.innerHTML = `
    <h2>${data.title}</h2>
    <img src="${data.img}" alt="${data.title}">
    <p>${data.desc}</p>
  `;
  document.getElementById('fieldworkGrid').style.display = 'none';
  document.getElementById('fieldworkDetail').style.display = 'block';
}

function returnToGrid() {
  document.getElementById('fieldworkGrid').style.display = 'grid';
  document.getElementById('fieldworkDetail').style.display = 'none';
}
</script>

