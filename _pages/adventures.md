---
permalink: /adventures/
title: "Adventures"
layout: single
classes: wide
---

<style>
/* Center map responsively */
.adventure-map {
  margin: 2rem auto;
  max-width: 800px;
  width: 100%;
}

.adventure-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
  gap: 1.25rem;
  margin-top: 2rem;
}

.adventure-card {
  background: #fff;
  border-radius: 8px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
  overflow: hidden;
  text-align: center;
  transition: transform 0.2s ease;
  cursor: pointer;
  text-decoration: none;
  color: inherit;
}
.adventure-card:hover {
  transform: scale(1.04);
}

.adventure-card img {
  width: 100%;
  height: 100px;
  object-fit: cover;
}

.adventure-card h4 {
  margin: 0.5rem;
  font-size: 0.95rem;
}
</style>

<div class="adventure-map">
  <iframe title="Country Highpoints &amp; Visits" aria-label="Map" id="datawrapper-chart-fCJW1" src="https://datawrapper.dwcdn.net/fCJW1/3/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="357" data-external="1"></iframe>
  <script type="text/javascript">
    !function(){
      "use strict";
      window.addEventListener("message",(function(a){
        if(void 0!==a.data["datawrapper-height"]){
          var e=document.querySelectorAll("iframe");
          for(var t in a.data["datawrapper-height"])
            for(var r,i=0;r=e[i];i++)
              if(r.contentWindow===a.source){
                var d=a.data["datawrapper-height"][t]+"px";
                r.style.height=d
              }
        }
      }))
    }();
  </script>
</div>

<div class="adventure-grid">
  <a href="/adventures/czechia/" class="adventure-card">
    <img src="/assets/images/flags/nepal.jpg" alt="Nepal">
    <h4>Czechia</h4>
  </a>

  <a href="/adventures/lithuania/" class="adventure-card">
    <img src="/assets/images/flags/chile.jpg" alt="Chile">
    <h4>Lithuania</h4>
  </a>

  <a href="/adventures/latvia/" class="adventure-card">
    <img src="/assets/images/flags/tanzania.jpg" alt="Tanzania">
    <h4>Latvia</h4>
  </a>

  <a href="/adventures/estonia/" class="adventure-card">
    <img src="/assets/images/flags/norway.jpg" alt="Norway">
    <h4>Estonia</h4>
  </a>

  <a href="/adventures/ghana/" class="adventure-card">
    <img src="/assets/images/flags/kazakhstan.jpg" alt="Kazakhstan">
    <h4>Ghana</h4>
  </a>

  <!-- Add more countries as needed -->
</div>

