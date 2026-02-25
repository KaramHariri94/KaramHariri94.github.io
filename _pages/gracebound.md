---
layout: single
title: "Gracebound"
permalink: /projects/gracebound/
author_profile: false
toc: true
toc_label: "Contents"
toc_icon: "gamepad"

# --- GALLERY CONFIGURATION ---
# Add your screenshots here. They will appear at the bottom.
gallery:
  - url: /assets/images/graceboundscreenshot1.png
    image_path: /assets/images/graceboundscreenshot1.png
    alt: "Gameplay Moment 1"
  - url: /assets/images/graceboundscreenshot2.png
    image_path: /assets/images/graceboundscreenshot2.png
    alt: "Gameplay Moment 2"
  - url: /assets/images/graceboundscreenshot3.png
    image_path: /assets/images/graceboundscreenshot3.png
    alt: "Gameplay Moment 3"
  - url: /assets/images/graceboundscreenshot4.png
    image_path: /assets/images/graceboundscreenshot4.png
    alt: "Gameplay Moment 4"
---

<a href="/" class="btn-back">
  <i class="fas fa-arrow-left"></i> Back
</a>

<div class="video-container">
  <video 
    autoplay 
    muted 
    loop 
    playsinline 
    controls 
    poster="/assets/images/gracebound_thumbnail.png"
    class="custom-video">
    <source src="/assets/videos/GraceboundVideo.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>
<br>

## What I Worked On

Modular AI Architecture: I engineered a scalable AI system using a custom Behavior Tree. I created a Base Enemy Class that has the common behavior between the different types which specific archetypes (Melee, Ranged, Explosive) inherit from and override their unique behaviors.

Animation Integration: I integrated the animation state machines for all archetypes, ensuring that logic states (like "Stunned" or "Attacking") stayed perfectly synced with visual feedback.

Data-Driven Design: To empower rapid iteration, I decoupled gameplay stats from logic using ScriptableObjects. This allowed designers to create multiple variants of the same enemy type with different difficulty levels without touching code.

Tactical Positioning System (EQS): To prevent enemies from "stacking" or forming a conga line, I implemented a custom Environmental Query System. Instead of pathfinding directly to the player, enemies identify and reserve Tactical Slots around the player. This forces the AI to flank and surround the target, creating dynamic pressure and encouraging player movement.

Combat Director (Token System): I developed a global manager that controls combat pacing. This system uses an Attack Token Pool to limit how many enemies can strike simultaneously, preventing the player from being unfairly overwhelmed while maintaining high encounter intensity.

Modular Enemy Spawner: I developed a designer-friendly spawner system that supports both Time-Based and Clear-Based waves. Designers can customize enemy types, wave counts, and spawn locations (either within a defined radius or at specific designated points).

Object Pooling: To ensure stable performance during high-intensity waves, the spawner utilizes a custom Object Pooler. This minimizes CPU spikes by recycling enemy actors instead of constantly instantiating and destroying them.

Camera Occlusion: I implemented a raycast-based occlusion system that detects geometry between the camera and the character, fading out walls or obstacles to keep the view clear.

<br>

## Gallery

{% include gallery caption="Screenshots from Gracebound" %}

<style>
  .video-container {
    position: relative;
    width: 100%;
    max-width: 100%;
    background: #000;
    border-radius: 8px;
    box-shadow: 0 0 20px rgba(0,0,0,0.5);
    overflow: hidden;
    /* This ensures the container holds the 16:9 shape before the video loads */
    aspect-ratio: 16 / 9; 
  }

  .custom-video {
    width: 100%;
    height: 100%;
    display: block;
    object-fit: cover; /* Ensures the video fills the area nicely */
  }

  /* Optional: Make the headers pop a bit more */
  h2 {
    border-bottom: 2px solid #1DE9B6;
    padding-bottom: 10px;
  }

  /* Back Button Desktop Styles */
  .btn-back {
    position: fixed; 
    top: 100px; /* Aligned with other pages */
    left: 20px;
    background-color: rgba(18, 18, 18, 0.8); 
    color: #fff !important;
    padding: 10px 20px;
    border-radius: 30px; 
    text-decoration: none !important;
    z-index: 99999 !important; /* Force on top */
    border: 1px solid #333;
    font-weight: bold;
    transition: all 0.3s ease;
    backdrop-filter: blur(5px); 
  }

  /* Hover Effect: Turns Teal */
  .btn-back:hover {
    background-color: #1DE9B6; 
    color: #000 !important;
    border-color: #1DE9B6;
    transform: translateX(-3px); 
  }

  /* --- MOBILE SPECIFIC STYLES --- */
  @media (max-width: 768px) {
    .btn-back {
      top: 10px;
      left: 10px;
      padding: 8px 15px;
      font-size: 0.9em;
    }
  } /* <--- CLOSED MOBILE SECTION HERE */

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