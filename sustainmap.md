---
layout: Page
title: Sustainability Map Project
subtitle: GEMS Society Event
permalink: /sustainmap.html
---


<style>
  :root{
    --page-col: #E6FFF7;         /* light green background */
    --text-col: #2C3E50;         /* dark blue-gray text */
    --link-col: #1E90FF;         /* blue links */
    --hover-col: #27AE60;        /* green hover */
    --navbar-col: #B3E5FC;       /* light blue navbar */ 
    --navbar-text-col: #2C3E50;  /* dark blue-gray navbar text */
    --navbar-border-col: #81D4FA;/* medium blue border */
    --footer-col: #B2DFDB;       /* light green footer */
    --footer-text-col: #2C3E50;  /* dark blue-gray footer text */
    --footer-link-col: #1E90FF;  /* blue footer links */
    --footer-hover-col: #27AE60; /* green footer hover */
    --max-width: 1000px;
  }

  html,body{
    height: 100%;
    margin: 0;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    background: var(--page-col);
    color: var(--text-col);
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }

  /* simple navbar */
  .site-nav{
    display:flex;
    align-items:center;
    justify-content:space-between;
    gap:1rem;
    /* use image instead of solid color - adjust the path if needed */
    background-image: url('/assets/green.png');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    color: var(--navbar-text-col);
    border-bottom: 1px solid var(--navbar-border-col);
    padding: .75rem 1rem;
    box-sizing: border-box;
  }
  .site-nav .brand{ font-weight:600; }
  .site-nav a{
    color: var(--navbar-text-col);
    text-decoration:none;
    margin-left:.5rem;
  }
  .site-nav a:hover{ color: var(--hover-col); }

  /* main wrapper */
  .sustain-map-wrapper{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-height: 70vh; /* keeps content vertically centered */
    padding: 2rem 1rem;
    box-sizing: border-box;
    max-width: var(--max-width);
    margin: 0 auto;
  }

  .sustain-map-title{
    text-align: center;
    margin: 0 0 1rem 0;
    font-size: 2rem;
    color: var(--text-col);
  }

  .map-container{
    width: 100%;
    max-width: var(--max-width);
    aspect-ratio: 16 / 9; /* keeps map responsive */
    box-shadow: 0 8px 24px rgba(0,0,0,0.12);
    border-radius: 8px;
    overflow: hidden;
    border: 1px solid rgba(0,0,0,0.06);
    background: #fff;
  }

  .map-container iframe{
    width: 100%;
    height: 100%;
    border: 0;
    display: block;
  }

  a, .link{
    color: var(--link-col);
  }
  a:hover, .link:hover{ color: var(--hover-col); }

  /* footer */
  .site-footer{
    background: var(--footer-col);
    color: var(--footer-text-col);
    padding: 1rem;
    text-align:center;
    margin-top: 2rem;
  }
  .site-footer a{ color: var(--footer-link-col); text-decoration:none; }
  .site-footer a:hover{ color: var(--footer-hover-col); }

  @media (max-width: 480px){
    .sustain-map-title{ font-size: 1.25rem; }
    .site-nav{ padding:.5rem; }
  }
</style>

<nav class="site-nav" role="navigation" aria-label="Main navigation">
  <div class="brand">GEMS Society</div>
  <div class="nav-links">
    <a href="/">Home</a>
    <a href="/events.html">Events</a>
    <a href="/contact.html">Contact</a>
  </div>
</nav>

<div class="sustain-map-wrapper" role="main" aria-labelledby="sustain-title">
  <h1 id="sustain-title" class="sustain-map-title">Sustainability Map</h1>

  <div class="map-container" role="region" aria-label="Sustainability map">
    <iframe src="https://www.google.com/maps/d/embed?mid=1vpPdS0OM4f2qios5Il8042YE1ZltnoA&ehbc=2E312F" allowfullscreen loading="lazy"></iframe>
  </div>
</div>
<style>
  /* ensure footer stays at the bottom of the viewport */
  html, body {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
  }
</style>

<footer class="site-footer" role="contentinfo" aria-label="Footer">
  <div>Part of the GEMS Society — <a href="/privacy.html">Privacy</a></div>
</footer>
