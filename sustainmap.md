---
layout: Page
title: Sustainability Map Project
subtitle: GEMS Society Event
permalink: /sustainmap.html
---

...existing code...
<style>
  .sustain-map-wrapper{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-height: 70vh; /* keeps content vertically centered */
    padding: 2rem 1rem;
    box-sizing: border-box;
  }

  .sustain-map-title{
    text-align: center;
    margin: 0 0 1rem 0;
    font-size: 2rem;
  }

  .map-container{
    width: 100%;
    max-width: 1000px;
    aspect-ratio: 16 / 9; /* keeps map responsive */
    box-shadow: 0 8px 24px rgba(0,0,0,0.12);
    border-radius: 8px;
    overflow: hidden;
  }

  .map-container iframe{
    width: 100%;
    height: 100%;
    border: 0;
    display: block;
  }

  @media (max-width: 480px){
    .sustain-map-title{ font-size: 1.25rem; }
  }
</style>

<div class="sustain-map-wrapper">
  <h1 class="sustain-map-title">Sustainability Map</h1>

  <div class="map-container" role="region" aria-label="Sustainability map">
    <iframe src="https://www.google.com/maps/d/embed?mid=1vpPdS0OM4f2qios5Il8042YE1ZltnoA&ehbc=2E312F" allowfullscreen loading="lazy"></iframe>
  </div>
</div>
