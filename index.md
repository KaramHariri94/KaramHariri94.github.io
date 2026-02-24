---
layout: splash
permalink: /
hidden: true

introduction:
  - image_path: /assets/images/bio-photo.jpg 
    alt: "Karam Hariri"
    title: "About Me"
    excerpt: |
      I am a Generalist Engineer with a passion for System Architecture. I don't just implement features; I build the ecosystems they live in.<br />
      My approach combines Modular AI that brings characters to life without tangling the codebase, Scalable Gameplay systems designed to grow from prototype to production, and custom Pipeline Tools that empower designers to iterate faster. I focus on writing clean, decoupled code that ensures the game is as fun to develop as it is to play.
      <br><br>
      **Skills & Tools:**<br>
      <div class="tech-stack">
        <img src="https://cdn.simpleicons.org/unrealengine/white" title="Unreal Engine" />
        <img src="https://cdn.simpleicons.org/unity/white" title="Unity" />
        <img src="https://cdn.simpleicons.org/cplusplus/00599C" title="C++" />
        <img src="https://cdn.simpleicons.org/csharp/239120" title="C#" />
        <img src="https://cdn.simpleicons.org/perforce/00B0E8" title="Perforce Helix" />
        <img src="https://cdn.simpleicons.org/github/white" title="GitHub" />
        <img src="https://cdn.simpleicons.org/visualstudio/5C2D91" title="Visual Studio" />
      </div>

# PROJECT 1
project_ai:
  - image_path: /assets/images/project1-thumb.jpg
    alt: "Modular AI System"
    title: "Modular AI System"
    excerpt: |
      A decoupled AI architecture using Behavior Trees. 
      Built for high-performance agent management. <br />
      ![Unreal](https://img.shields.io/badge/-Unreal-313131?style=flat&logo=unreal-engine&logoColor=white)
      ![C++](https://img.shields.io/badge/-C++-00599C?style=flat&logo=c%2B%2B&logoColor=white)
    url: "/projects/modular-ai-system/"
    btn_label: "View Case Study"
    btn_class: "btn--primary"

# PROJECT 2
project_combat:
  - image_path: /assets/images/project2-thumb.jpg
    alt: "Combat Prototype"
    title: "Combat Prototype"
    excerpt: |
      Fast-paced melee combat system with hit-stop and camera shake. 
      Focused on 3C (Character, Controls, Camera). <br />
      ![Unity](https://img.shields.io/badge/-Unity-100000?style=flat&logo=unity&logoColor=white)
      ![C#](https://img.shields.io/badge/-C%23-239120?style=flat&logo=c-sharp&logoColor=white)
    url: "/projects/combat-prototype/"
    btn_label: "View Case Study"
    btn_class: "btn--primary"
---

<style>
  /* --- 1. RESET PAGE PADDING --- */
  /* This removes the white gap between the top line (nav) and your bio */
  .page__content {
    padding-top: 0 !important;
  }

  /* --- 2. BIO SECTION (THE BLACK BOX) --- */
  .bio-wrapper {
    background-color: #121212;
    color: white !important;
    padding: 60px 0; /* Vertical breathing room */
    
    /* BREAKOUT LOGIC: Makes the background go edge-to-edge horizontally */
    width: 100vw;
    position: relative;
    left: 50%;
    right: 50%;
    margin-left: -50vw;
    margin-right: -50vw;
    
    /* NO NEGATIVE MARGIN: This stops it from going "up" into the tabs */
    margin-top: 0; 
  }

  /* --- 3. INNER CONTENT CONSTRAINT --- */
  /* Keeps your text and face centered, not stretched to the edges */
  .bio-wrapper .feature__wrapper {
    max-width: 1280px; 
    margin: 0 auto;
    padding-left: 2em;
    padding-right: 2em;
  }

  /* --- 4. PROFILE PICTURE --- */
  .bio-wrapper .feature__item-teaser img {
    border-radius: 50% !important;
    width: 250px !important;
    height: 250px !important;
    object-fit: cover;
    border: 3px solid #1DE9B6;
    box-shadow: 0 0 15px rgba(0,0,0,0.5);
  }

  /* --- 5. TECH STACK ICONS --- */
  .tech-stack {
    display: flex;
    gap: 15px;
    margin-top: 20px;
    flex-wrap: wrap;
    align-items: center;
  }

  .tech-stack img {
    width: 32px !important;  
    height: 32px !important;
    border-radius: 0 !important;
    border: none !important;
    background: none !important;
    box-shadow: none !important;
    padding: 0 !important;
    margin: 0 !important;
  }

  /* --- 6. TEXT COLOR OVERRIDES --- */
  .bio-wrapper .feature__item-title, 
  .bio-wrapper .feature__item-excerpt {
    color: white !important;
  }
  
  /* Remove default bottom margin from the bio row to stop it pushing down too far */
  .bio-wrapper .feature__row {
      margin-bottom: 0 !important;
  }
</style>

<div class="bio-wrapper">
  {% include feature_row id="introduction" type="left" %}
</div>

<div id="projects" class="container">
  <h2 style="text-align: center; margin-top: 50px;">📂 Selected Projects</h2>
  
  {% include feature_row id="project_ai" type="left" %}
  <hr>
  {% include feature_row id="project_combat" type="right" %}
</div>