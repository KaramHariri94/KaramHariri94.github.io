---
layout: single
title: "CastByLight"
permalink: /projects/castbylight/
author_profile: false
toc: true
toc_label: "Contents"
toc_icon: "gamepad"

# --- GALLERY CONFIGURATION ---
# Add your screenshots here. They will appear at the bottom.
gallery:
  - url: /assets/images/castbylightscreenshot1.png
    image_path: /assets/images/castbylightscreenshot1.png
    alt: "Gameplay Moment 1"
  - url: /assets/images/castbylightscreenshot2.png
    image_path: /assets/images/castbylightscreenshot2.png
    alt: "Gameplay Moment 2"
  - url: /assets/images/Castbylight.JPG
    image_path: /assets/images/Castbylight.JPG
    alt: "Award"
  - url: /assets/images/castbylightscreenshot4.jpg
    image_path: /assets/images/castbylightscreenshot4.jpg
    alt: "Arcade"
  
---

<div class="video-container">
  <iframe 
    src="https://www.youtube.com/embed/BH-QS6EvlBg?playlist=BH-QS6EvlBg&loop=1&autoplay=1&mute=1&controls=1"
    title="Youtube video player"
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope" 
    allowfullscreen>
  </iframe>
</div>

<br>

## What I Worked On

During this project I developed a 2D character controller handling all player traversal states. This included implementing the logic for movement, jumping, and ladder climbing, as well as integrating the animation state machine to ensure fluid transitions between actions.

Sun & Shadow Mechanics (Bezier Curves) I implemented the sun rotation by using Bezier Curves to calculate the sun's trajectory, allowing for smooth, non-linear movement that dynamically shifts shadows, which the player uses to traverse the environment.

Level Implementation I acted as the bridge between design and art. I was responsible for assembling the game levels within Unity, integrating assets provided by the artists, and helped with setting up the logic flows designed by the level designers.

Moreover, I implemented Scene Management system to handle level loading, unloading, and transitions, ensuring a seamless experience between different stages of the game.

<br>

## 📸 Gallery

{% include gallery caption="Screenshots from CastByLight" %}

<style>
  /* Makes the video responsive and centered */
  .video-container {
    position: relative;
    padding-bottom: 56.25%; /* 16:9 Aspect Ratio */
    height: 0;
    overflow: hidden;
    max-width: 100%;
    background: #000;
    border-radius: 8px;
    box-shadow: 0 0 20px rgba(0,0,0,0.5);
  }
  
  .video-container iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }

  /* Optional: Make the headers pop a bit more */
  h2 {
    border-bottom: 2px solid #1DE9B6;
    padding-bottom: 10px;
  }
</style>