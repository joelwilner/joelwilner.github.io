---
permalink: /research/
title: "Research"
layout: single
classes: wide
---

<style>
.research-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 1.5rem;
  padding-bottom: 2rem;
}

.research-card {
  background: #fff;
  border-radius: 10px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
  overflow: hidden;
  cursor: pointer;
  transition: transform 0.2s ease;
}
.research-card:hover {
  transform: scale(1.02);
}

.research-card img {
  width: 100%;
  height: 120px;
  object-fit: cover;
}

.research-content {
  padding: 0.75rem;
}

.research-content h3 {
  font-size: 1rem;
  margin: 0 0 0.5rem 0;
}

/* Detail View */
#researchDetail {
  padding: 1rem;
  background: #fff;
  border-radius: 10px;
  box-shadow: 0 0 8px rgba(0,0,0,0.1);
  margin-top: 2rem;
}

#researchDetail button {
  margin-bottom: 1rem;
  background: none;
  font-size: 1rem;
  cursor: pointer;
  padding: 0;
  color: #007acc;
}
#researchDetail button:hover {
  text-decoration: underline;
}

/* Flex layout for detail view */
.detail-flex {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

@media (min-width: 768px) {
  .detail-flex {
    flex-direction: row;
    align-items: flex-start;
  }

  .detail-flex img {
    width: 40%;
    max-width: 400px;
    height: auto;
    border-radius: 8px;
    margin-right: 1.5rem;
  }

  .detail-text {
    flex: 1;
  }
}

@media (max-width: 767px) {
  .detail-flex img {
    width: 100%;
    max-height: 300px;
    object-fit: cover;
    border-radius: 8px;
  }
}
</style>

<!-- Grid of Fieldwork Cards -->
<div id="researchGrid" class="fieldwork-grid">

  <div class="research-card" onclick="showDetail('site-a')">
    <img src="/assets/images/project2.jpg" alt="Site A">
    <div class="research-content">
      <h3>Paramo de Frontino, Colombia</h3>
    </div>
  </div>

  <div class="research-card" onclick="showDetail('site-b')">
    <img src="/assets/images/Russell.jpg" alt="Site B">
    <div class="research-content">
      <h3>Russell Glacier, Greenland</h3>
    </div>
  </div>

  <div class="research-card" onclick="showDetail('site-c')">
    <img src="/assets/images/project3.png" alt="Site C">
    <div class="research-content">
      <h3>Summit Station, Greenland</h3>
    </div>
  </div>

</div>

<!-- Detail View -->
<div id="researchDetail" style="display: none;">
  <button onclick="returnToGrid()">← Back to Fieldwork</button>
  <div id="detailContent" class="detail-flex"></div>
</div>

<script>
const researchData = {
  'site-a': {
    title: 'Paramo de Frontino, Colombia',
    img: '/assets/images/project2.jpg',
    desc: 'Boulder sampling for cosmogenic surface exposure dating to reconstruct the glacial history of a high-altitude paramo in the Colombian Andes.'
  },
  'site-b': {
    title: 'Russell Glacier, Greenland',
    img: '/assets/images/Russell.jpg',
    desc: 'Annual time-lapse photography to elucidate the effects of fluvial dynamics on calving at the glacier terminus.'
  },
  'site-c': {
    title: 'Summit Station, Greenland',
    img: '/assets/images/ApRES.jpg',
    desc: 'Autonomous phase-sensitive radio-echo sounder (ApRES) deployment for firn densification and dynamic strain components of surface elevation change.'
  }
};

function showDetail(key) {
  const data = researchData[key];
  const container = document.getElementById('detailContent');
  container.innerHTML = `
    <div class="detail-flex">
      <img src="${data.img}" alt="${data.title}">
      <div class="detail-text">
        <h2>${data.title}</h2>
        <p>${data.desc}</p>
      </div>
    </div>
  `;
  document.getElementById('researchGrid').style.display = 'none';
  document.getElementById('researchDetail').style.display = 'block';
}

function returnToGrid() {
  document.getElementById('researchGrid').style.display = 'grid';
  document.getElementById('researchDetail').style.display = 'none';
}
</script>

