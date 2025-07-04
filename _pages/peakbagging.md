---
permalink: /peakbagging/
title: "Adventures"
layout: single
classes: wide
---

<style>
.tabs {
  display: flex;
  margin-bottom: 1rem;
  border-bottom: 2px solid #ddd;
}
.tab {
  padding: 0.75rem 1.25rem;
  cursor: pointer;
  font-weight: 600;
  border-bottom: 3px solid transparent;
  transition: border-color 0.3s ease;
}
.tab.active {
  border-color: #222;
}
.tab-content {
  display: none;
}
.tab-content.active {
  display: block;
}
.adventure-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
  gap: 1rem;
  margin-top: 1rem;
}
.adventure-card {
  text-align: center;
  background: #fff;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
  transition: transform 0.2s ease;
}
.adventure-card:hover {
  transform: scale(1.03);
}
.adventure-card img {
  width: 100%;
  height: 120px;
  object-fit: cover;
}
</style>

<!-- Tabs -->
<div class="tabs">
  <div class="tab active" onclick="showTab('countries')">Country Highpoints</div>
  <div class="tab" onclick="showTab('states')">State Highpoints</div>
</div>

<!-- Country Highpoints -->
<div id="tab-countries" class="tab-content active">
  <iframe title="Country Highpoints &amp; Visits" aria-label="Map" id="datawrapper-chart-fCJW1" src="https://datawrapper.dwcdn.net/fCJW1/3/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="357" data-external="1"></iframe>
  <script type="text/javascript">
    !function(){
      "use strict";
      window.addEventListener("message",function(a){
        if(void 0!==a.data["datawrapper-height"]){
          var e=document.querySelectorAll("iframe");
          for(var t in a.data["datawrapper-height"])
            for(var r,i=0;r=e[i];i++)
              if(r.contentWindow===a.source){
                r.style.height=a.data["datawrapper-height"][t]+"px";
              }
        }
      });
    }();
  </script>
<p>Coming soon: Trip reports for each country highpoint.</p>
  <div class="adventure-grid">
    <!-- Insert full country cards here, e.g. Czechia to Tanzania -->
    <!-- Example below -->
      <a href="/adventures/czechia/" class="adventure-card">
    <img src="/assets/images/highpoints/Czechia.jpg" loading="lazy" alt="Czechia">
    <h4>39. Czechia</h4>
  </a>

  <a href="/adventures/lithuania/" class="adventure-card">
    <img src="/assets/images/highpoints/Lithuania.jpg" loading="lazy" alt="Lithuania">
    <h4>38. Lithuania</h4>
  </a>

  <a href="/adventures/latvia/" class="adventure-card">
    <img src="/assets/images/highpoints/Latvia.jpg" loading="lazy" alt="Latvia">
    <h4>37. Latvia</h4>
  </a>

  <a href="/adventures/estonia/" class="adventure-card">
    <img src="/assets/images/highpoints/Estonia.jpg" loading="lazy" alt="Estonia">
    <h4>36. Estonia</h4>
  </a>

  <a href="/adventures/ghana/" class="adventure-card">
    <img src="/assets/images/highpoints/Ghana.jpg" loading="lazy" alt="Ghana">
    <h4>35. Ghana</h4>
  </a>

  <a href="/adventures/togo/" class="adventure-card">
    <img src="/assets/images/highpoints/Togo.jpg" loading="lazy" alt="Togo">
    <h4>34. Togo</h4>
  </a>

  <a href="/adventures/benin/" class="adventure-card">
    <img src="/assets/images/highpoints/Benin.jpg" loading="lazy" alt="Benin">
    <h4>33. Benin</h4>
  </a>

  <a href="/adventures/malta/" class="adventure-card">
    <img src="/assets/images/highpoints/Malta.jpg" loading="lazy" alt="Malta">
    <h4>32. Malta</h4>
  </a>

  <a href="/adventures/vatican-city/" class="adventure-card">
    <img src="/assets/images/highpoints/VaticanCity.jpg" loading="lazy" alt="Vatican City">
    <h4>31. Vatican City</h4>
  </a>

  <a href="/adventures/san-marino/" class="adventure-card">
    <img src="/assets/images/highpoints/SanMarino.jpg" loading="lazy" alt="San Marino">
    <h4>30. San Marino</h4>
  </a>

  <a href="/adventures/monaco/" class="adventure-card">
    <img src="/assets/images/highpoints/Monaco.jpg" loading="lazy" alt="Monaco">
    <h4>29. Monaco</h4>
  </a>

  <a href="/adventures/liechtenstein/" class="adventure-card">
    <img src="/assets/images/highpoints/Liechtenstein.jpg" loading="lazy" alt="Liechtenstein">
    <h4>28. Liechtenstein</h4>
  </a>

  <a href="/adventures/belize/" class="adventure-card">
    <img src="/assets/images/highpoints/Belize.jpg" loading="lazy" alt="Belize">
    <h4>27. Belize</h4>
  </a>

  <a href="/adventures/antigua-barbuda/" class="adventure-card">
    <img src="/assets/images/highpoints/AntiguaBarbuda.jpg" loading="lazy" alt="Antigua and Barbuda">
    <h4>26. Antigua & Barbuda</h4>
  </a>

  <a href="/adventures/saint-kitts-nevis/" class="adventure-card">
    <img src="/assets/images/highpoints/SaintKittsNevis.jpg" loading="lazy" alt="Saint Kitts and Nevis">
    <h4>25. Saint Kitts & Nevis</h4>
  </a>

  <a href="/adventures/netherlands/" class="adventure-card">
    <img src="/assets/images/highpoints/Netherlands.jpg" loading="lazy" alt="Netherlands">
    <h4>24. Netherlands</h4>
  </a>

  <a href="/adventures/grenada/" class="adventure-card">
    <img src="/assets/images/highpoints/Grenada.jpg" loading="lazy" alt="Grenada">
    <h4>23. Grenada</h4>
  </a>

  <a href="/adventures/united-kingdom/" class="adventure-card">
    <img src="/assets/images/highpoints/UnitedKingdom.jpg" loading="lazy" alt="United Kingdom">
    <h4>22. United Kingdom</h4>
  </a>

  <a href="/adventures/belgium/" class="adventure-card">
    <img src="/assets/images/highpoints/Belgium.jpg" loading="lazy" alt="Belgium">
    <h4>21. Belgium</h4>
  </a>

  <a href="/adventures/luxembourg/" class="adventure-card">
    <img src="/assets/images/highpoints/Luxembourg.jpg" loading="lazy" alt="Luxembourg">
    <h4>20. Luxembourg</h4>
  </a>

  <a href="/adventures/hungary/" class="adventure-card">
    <img src="/assets/images/highpoints/Hungary.jpg" loading="lazy" alt="Hungary">
    <h4>19. Hungary</h4>
  </a>

  <a href="/adventures/poland/" class="adventure-card">
    <img src="/assets/images/highpoints/Poland.jpg" loading="lazy" alt="Poland">
    <h4>18. Poland</h4>
  </a>

  <a href="/adventures/slovakia/" class="adventure-card">
    <img src="/assets/images/highpoints/Slovakia.jpg" loading="lazy" alt="Slovakia">
    <h4>17. Slovakia</h4>
  </a>

  <a href="/adventures/denmark/" class="adventure-card">
    <img src="/assets/images/highpoints/Denmark.jpg" loading="lazy" alt="Denmark">
    <h4>16. Denmark</h4>
  </a>

  <a href="/adventures/sweden/" class="adventure-card">
    <img src="/assets/images/highpoints/Sweden.jpg" loading="lazy" alt="Sweden">
    <h4>15. Sweden</h4>
  </a>

  <a href="/adventures/norway/" class="adventure-card">
    <img src="/assets/images/highpoints/Norway.jpg" loading="lazy" alt="Norway">
    <h4>14. Norway</h4>
  </a>

  <a href="/adventures/cabo-verde/" class="adventure-card">
    <img src="/assets/images/highpoints/CaboVerde.jpg" loading="lazy" alt="Cabo Verde">
    <h4>13. Cabo Verde</h4>
  </a>

  <a href="/adventures/portugal/" class="adventure-card">
    <img src="/assets/images/highpoints/Portugal.jpg" loading="lazy" alt="Portugal">
    <h4>12. Portugal</h4>
  </a>

  <a href="/adventures/dominican-republic/" class="adventure-card">
    <img src="/assets/images/highpoints/DominicanRepublic.jpg" loading="lazy" alt="Dominican Republic">
    <h4>11. Dominican Republic</h4>
  </a>

  <a href="/adventures/ireland/" class="adventure-card">
    <img src="/assets/images/highpoints/Ireland.jpg" loading="lazy" alt="Ireland">
    <h4>10. Ireland</h4>
  </a>

  <a href="/adventures/mexico/" class="adventure-card">
    <img src="/assets/images/highpoints/Mexico.jpg" loading="lazy" alt="Mexico">
    <h4>9. Mexico</h4>
  </a>

  <a href="/adventures/bulgaria/" class="adventure-card">
    <img src="/assets/images/highpoints/Bulgaria.jpg" loading="lazy" alt="Bulgaria">
    <h4>8. Bulgaria</h4>
  </a>

  <a href="/adventures/albania-north-macedonia/" class="adventure-card">
    <img src="/assets/images/highpoints/AlbaniaNorthMacedonia.jpg" loading="lazy" alt="Albania & North Macedonia">
    <h4>7–6. Albania & North Macedonia</h4>
  </a>

  <a href="/adventures/kosovo/" class="adventure-card">
    <img src="/assets/images/highpoints/Kosovo.jpg" loading="lazy" alt="Kosovo">
    <h4>5. Kosovo</h4>
  </a>

  <a href="/adventures/serbia/" class="adventure-card">
    <img src="/assets/images/highpoints/Serbia.jpg" loading="lazy" alt="Serbia">
    <h4>4. Serbia</h4>
  </a>

  <a href="/adventures/finland/" class="adventure-card">
    <img src="/assets/images/highpoints/Finland.jpg" loading="lazy" alt="Finland">
    <h4>3. Finland</h4>
  </a>

  <a href="/adventures/saint-lucia/" class="adventure-card">
    <img src="/assets/images/highpoints/SaintLucia.jpg" loading="lazy" alt="Saint Lucia">
    <h4>2. Saint Lucia</h4>
  </a>

  <a href="/adventures/tanzania/" class="adventure-card">
    <img src="/assets/images/highpoints/Tanzania.jpg" loading="lazy" alt="Tanzania">
    <h4>1. Tanzania</h4>
  </a>
  </div>
</div>

<!-- State Highpoints -->
<div id="tab-states" class="tab-content">
  <p>Coming soon: Interactive map and write-ups from all 50 U.S. state highpoints.</p>
  <div class="adventure-grid">
  <!--  <a href="/adventures/denali/" class="adventure-card">
      <img src="/assets/images/state-highpoints/Denali.jpg" loading="lazy" alt="Denali">
      <h4>Alaska – Denali</h4>
    </a>
    <a href="/adventures/whitney/" class="adventure-card">
      <img src="/assets/images/state-highpoints/Whitney.jpg" loading="lazy" alt="Mount Whitney">
      <h4>California – Whitney</h4>
    </a> -->
    <!-- Add more state cards here -->
  </div>
</div>

<script>
function showTab(tabName) {
  const tabs = document.querySelectorAll(".tab");
  const contents = document.querySelectorAll(".tab-content");
  tabs.forEach(t => t.classList.remove("active"));
  contents.forEach(c => c.classList.remove("active"));
  document.querySelector(`.tab[onclick="showTab('${tabName}')"]`).classList.add("active");
  document.getElementById(`tab-${tabName}`).classList.add("active");
}
</script>

