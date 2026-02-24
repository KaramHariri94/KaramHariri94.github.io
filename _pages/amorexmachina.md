---
layout: single
title: "AmoreExMachina"
permalink: /projects/amorexmachina/
author_profile: false
toc: true
toc_label: "Contents"
toc_icon: "gamepad"

# --- GALLERY CONFIGURATION ---
# Add your screenshots here. They will appear at the bottom.
gallery:
  - url: /assets/images/amorexmachinascreenshot1.png
    image_path: /assets/images/amorexmachinascreenshot1.png
    alt: "Gameplay Moment 1"
  - url: /assets/images/amorexmachinascreenshot2.png
    image_path: /assets/images/amorexmachinascreenshot2.png
    alt: "Gameplay Moment 2"
  - url: /assets/images/amorexmachinascreenshot3.png
    image_path: /assets/images/amorexmachinascreenshot3.png
    alt: "Gameplay Moment 3"
  - url: /assets/images/amorexmachinascreenshot4.png
    image_path: /assets/images/amorexmachinascreenshot4.png
    alt: "Gameplay Moment 4"
---

<div class="video-container">
  <iframe 
    src="https://www.youtube.com/embed/nVCMtpdZYTk?playlist=nVCMtpdZYTk&loop=1&autoplay=1&mute=1&controls=1" 
    title="YouTube video player"
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
    allowfullscreen>
  </iframe>
</div>

<div style="text-align: center; margin-top: 20px; margin-bottom: 30px;">
  <a href="https://amor-ex-machina.itch.io/" class="btn btn--primary btn--large" target="_blank">
    <i class="fab fa-itch-io"></i> Play on Itch.io
  </a>
</div>

<br>

## What I Worked On

AI Behavior Trees: I designed and implemented the enemy AI architecture using **Behavior Trees**. This system managed patrol paths, detection states, and the reaction logic, allowing guards to investigate distractions and respond to the player's presence dynamically.

Stealth & Possession Mechanics: I developed the core "Hostile Takeover" mechanic, allowing the player to hack and overtake enemy guards. This involved complex state handling to seamlessly switch control between the main character and the possessed NPC, enabling the player to lure other guards out of position.

Character Movement & Camera transition: I implemented the foundational character controller, ensuring smooth movement and interaction responsiveness, which is critical for a precision stealth game. Moreover, I implemented the camera logic responsible for the possession sequence. I programmed a smooth transition that interpolates from the player's Third-Person camera to the enemy's First-Person view. This visual shift was critical for selling the "hack" effect and immediately orienting the player inside the new body.

Technical Art (Shaders & Lighting): I contributed to the visual fidelity of the project by writing custom Shaders and configuring lighting setups. This work was essential for establishing the game's moody atmosphere and providing visual cues for the stealth mechanics.

<br>

## Gallery

{% include gallery caption="Screenshots from AmorExMachina" %}

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