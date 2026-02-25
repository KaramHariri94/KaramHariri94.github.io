---
layout: single
title: "Resume"
permalink: /resume/
author_profile: false
---

<a href="/" class="btn-back">
  <i class="fas fa-arrow-left"></i> Back
</a>

<div class="resume-container">
  <iframe 
    src="/assets/images/Karam_Hariri_CV.pdf" 
    width="100%" 
    height="1000px" 
    style="border: none; border-radius: 8px; box-shadow: 0 0 20px rgba(0,0,0,0.2);">
  </iframe>
</div>

<div style="text-align: center; margin-top: 30px;">
  <a href="/assets/docs/Karam_Hariri_CV.pdf" class="btn btn--primary btn--large" download>
    <i class="fas fa-file-download"></i> Download PDF
  </a>
</div>

<style>
  .resume-container {
    width: 100%;
    height: 1050px;
    margin-top: 20px;
  }

  /* Back Button styling to match your projects */
  .btn-back {
    position: fixed; 
    top: 80px;
    left: 20px;
    background-color: rgba(18, 18, 18, 0.8); 
    color: #fff !important;
    padding: 10px 20px;
    border-radius: 30px; 
    text-decoration: none !important;
    z-index: 99999 !important;
    border: 1px solid #333;
    font-weight: bold;
    transition: all 0.3s ease;
    backdrop-filter: blur(5px);
  }

  .btn-back:hover {
    background-color: #1DE9B6; 
    color: #000 !important;
    border-color: #1DE9B6;
    transform: translateX(-3px); 
  }

  @media (max-width: 768px) {
    .resume-container {
      height: 600px;
    }
    .btn-back {
      top: 10px;
      left: 10px;
      padding: 8px 15px;
      font-size: 0.9em;
    }
  }

  /* --- GLOBAL FOOTER STYLES (Desktop & Mobile) --- */
  .page__footer-follow a[href*="feed"],
  .page__footer-follow a[href*=".xml"],
  .fa-rss-square {
    display: none !important;
  }

  /* Hide the Copyright text */
  .page__footer-copyright {
    display: none !important;
  }

  /* Center the Icons */
  .page__footer-follow {
    text-align: center !important;
    display: block !important;
    width: 100% !important;
  }

  .page__footer-follow ul.social-icons {
    display: inline-block !important;
    margin: 0 auto !important;
    padding: 0 !important;
    float: none !important;
  }
</style>