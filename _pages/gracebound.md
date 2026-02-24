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
  - url: /assets/images/project1-thumb.jpg
    image_path: /assets/images/project1-thumb.jpg
    alt: "Gameplay Moment 1"
  - url: /assets/images/project1-thumb.jpg
    image_path: /assets/images/project1-thumb.jpg
    alt: "Gameplay Moment 2"
  - url: /assets/images/project1-thumb.jpg
    image_path: /assets/images/project1-thumb.jpg
    alt: "Gameplay Moment 3"
---

<br>

## What I Worked On

Modular AI Architecture: I engineered a scalable AI system using a custom Behavior Tree. I created a Base Enemy Class that has the common behavior between the different types which specific archetypes (Melee, Ranged, Explosive) inherit from and override their unique behaviors. To empower design iteration, I decoupled stats from logic using ScriptableObjects, allowing designers to create different types of the same enemy with different stats. I also integrated the animation state machines for all enemy types to ensure fluid combat feedback

Tactical Positioning System (EQS) To prevent enemies from "stacking" or forming a conga line, I implemented a custom Environmental Query System. Instead of pathfinding directly to the player, enemies identify and reserve Tactical Slots around the player. This forces the AI to flank and surround the target, creating dynamic pressure and encouraging player movement.

Combat Director (Token System) I developed a global manager that controls combat pacing. This system uses an Attack Token Pool to limit how many enemies can strike simultaneously, preventing the player from being unfairly overwhelmed while maintaining high encounter intensity.

Camera Occlusion & Animation I implemented a raycast-based occlusion system that detects geometry between the camera and the character, fading out walls or obstacles to keep the view clear.

<br>

## Gallery

{% include gallery caption="Screenshots from Gracebound" %}

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