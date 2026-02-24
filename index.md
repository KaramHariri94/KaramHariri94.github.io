---
layout: splash
permalink: /
hidden: true

introduction:
  - image_path: /assets/images/bio-photo.jpg 
    alt: "Karam Hariri"
    title: "About Me"
    excerpt: |
      **Generalist Game Programmer | System Architect** <br />
      I build robust tools and gameplay systems that help designers work faster.
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
  /* --- BIO SECTION WRAPPER --- */
  .bio-wrapper {
    background-color: #121212;
    color: white !important;
    padding: 50px 0;
    margin-top: -2em;
  }

  /* --- TARGET THE PROFILE PICTURE ONLY --- */
  .bio-wrapper .feature__item-teaser img {
    border-radius: 50% !important;
    width: 250px !important;
    height: 250px !important;
    object-fit: cover;
    border: 3px solid #1DE9B6;
    box-shadow: 0 0 15px rgba(0,0,0,0.5);
  }

  /* --- TECH STACK ICONS (SQUARE & SMALL) --- */
  .tech-stack {
    display: flex; /* Forces horizontal row */
    gap: 12px;     /* Space between icons */
    margin-top: 15px;
    flex-wrap: wrap;
    align-items: center;
  }

  .tech-stack img {
    width: 32px !important;  
    height: 32px !important;
    border-radius: 0 !important; /* Forces icons to be square */
    border: none !important;
    background: none !important;
    box-shadow: none !important;
  }

  .bio-wrapper .feature__item-title, 
  .bio-wrapper .feature__item-excerpt {
    color: white !important;
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