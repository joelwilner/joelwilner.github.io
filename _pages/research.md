---
permalink: /research/
title: "Research"
layout: single
classes: wide
---

<style>
.research-carousel-wrapper {
  position: relative;
  overflow: hidden;
}

.research-carousel {
  display: flex;
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  gap: 1rem;
  padding-bottom: 1rem;
  scroll-behavior: smooth;
}

.research-card {
  flex: 0 0 auto;
  width: 220px;
  border-radius: 10px;
  background: #fff;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
  scroll-snap-align: start;
}

.research-card img {
  width: 100%;
  height: 120px;
  object-fit: cover;
  border-top-left-radius: 10px;
  border-top-right-radius: 10px;
}

.research-content {
  padding: 0.75rem;
}

.research-content h3 {
  font-size: 1rem;
  margin: 0 0 0.5rem 0;
}

.research-nav {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  width: 2rem;
  height: 2rem;
  background: rgba(0,0,0,0.4);
  color: white;
  border: none;
  border-radius: 50%;
  cursor: pointer;
  z-index: 10;
}
.research-nav.left {
  left: 0.5rem;
}
.research-nav.right {
  right: 0.5rem;
}
</style>

<div class="research-carousel-wrapper">
  <button class="research-nav left" onclick="scrollResearch(-1)">&#8249;</button>
  <button class="research-nav right" onclick="scrollResearch(1)">&#8250;</button>

  <div class="research-carousel" id="researchCarousel">

  <div class="research-card">
    <img src="/assets/images/project1.jpg" alt="Project 1">
    <div class="research-content">
      <h3>Project One</h3>
      <p>Brief description of Project One.</p>
    </div>
  </div>

  <div class="research-card">
    <img src="/assets/images/project2.jpg" alt="Project 2">
    <div class="research-content">
      <h3>Project Two</h3>
      <p>Brief description of Project Two.</p>
    </div>
  </div>

  <div class="research-card">
    <img src="/assets/images/project3.png" alt="Project 3">
    <div class="research-content">
      <h3>Project Three</h3>
      <p>Brief description of Project Three.</p>
    </div>
  </div>

  <!-- Add more cards as needed -->

  </div>
</div>

<script>
function scrollResearch(direction) {
  const container = document.getElementById('researchCarousel');
  const scrollAmount = 240;
  container.scrollBy({ left: direction * scrollAmount, behavior: 'smooth' });
}
</script>

