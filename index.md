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
      **Tech Stack:**<br>
      ![C++](https://img.shields.io/badge/-C++-00599C?style=flat&logo=c%2B%2B&logoColor=white)
      ![C#](https://img.shields.io/badge/-C%23-239120?style=flat&logo=c-sharp&logoColor=white)
      ![Unity](https://img.shields.io/badge/-Unity-100000?style=flat&logo=unity&logoColor=white)
      ![Unreal](https://img.shields.io/badge/-Unreal-313131?style=flat&logo=unreal-engine&logoColor=white)

# PROJECT 1
project_ai:
  - image_path: /assets/images/project1-thumb.jpg
    alt: "Modular AI System"
    title: "Modular AI System"
    excerpt: >
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
    excerpt: >
      Fast-paced melee combat system with hit-stop and camera shake. 
      Focused on 3C (Character, Controls, Camera). <br />
      ![Unity](https://img.shields.io/badge/-Unity-100000?style=flat&logo=unity&logoColor=white)
      ![C#](https://img.shields.io/badge/-C%23-239120?style=flat&logo=c-sharp&logoColor=white)
    url: "/projects/combat-prototype/"
    btn_label: "View Case Study"
    btn_class: "btn--primary"

---

<style>
  /* This makes the top section dark */
  .bio-wrapper {
    background-color: #121212;
    color: white !important;
    padding: 60px 0;
    margin-top: -2em; /* Removes gap at top */
  }
  
  /* Forces circular image */
  .bio-wrapper img {
    border-radius: 50% !important;
    width: 250px !important;
    height: 250px !important;
    object-fit: cover;
    border: 3px solid #1DE9B6;
  }

  /* Ensures text is white in dark section */
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