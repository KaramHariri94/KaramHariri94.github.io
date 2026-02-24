---
layout: splash
permalink: /
hidden: true

introduction:
  - image_path: /assets/images/Image1.png
    alt: "Karam Hariri"
    title: "About Me"
    excerpt: |
      I am a Generalist Engineer with a passion for System Architecture. I don't just implement features; I build the ecosystems they live in.<br />
      My approach combines Modular AI that brings characters to life without tangling the codebase, Scalable Gameplay systems designed to grow from prototype to production, and custom Pipeline Tools that empower designers to iterate faster. I focus on writing clean, decoupled code that ensures the game is as fun to develop as it is to play.
      <br><br>
      <br>
      <div class="tech-stack">
        <img src="https://cdn.simpleicons.org/unrealengine/white" title="Unreal Engine" />
        
        <img src="https://cdn.simpleicons.org/unity/white" title="Unity" />
        
        <img src="https://cdn.simpleicons.org/cplusplus/00599C" title="C++" />
        
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg" title="C#" />
        
        <img src="https://cdn.simpleicons.org/perforce/00B0E8" title="Perforce Helix" />
        
        <img src="https://cdn.simpleicons.org/github/white" title="GitHub" />
        
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/visualstudio/visualstudio-original.svg" title="Visual Studio" />
      </div>

# ![Unreal](https://img.shields.io/badge/-Unreal-313131?style=flat&logo=unreal-engine&logoColor=white)
# ![C++](https://img.shields.io/badge/-C++-00599C?style=flat&logo=c%2B%2B&logoColor=white)
# ![Unity](https://img.shields.io/badge/-Unity-100000?style=flat&logo=unity&logoColor=white)
# ![C#](https://img.shields.io/badge/-C%23-239120?style=flat&logo=c-sharp&logoColor=white)
# <br><br>
# <strong>Tech:</strong>
# <div class="tech-stack">
# <img src="https://cdn.simpleicons.org/unrealengine/000000" title="Unreal Engine" />
# <img src="https://cdn.simpleicons.org/cplusplus/00599C" title="C++" />
# </div>

# PROJECT 1
project_Gracebound:
  - image_path: /assets/images/project1-thumb.jpg
    alt: "Gracebound"
    title: "Gracebound"
    excerpt: |
      A fast-paced hack-and-slash where you fight to save the world, only to realize you were bringing its demise.<br />
      <br><br>
      <div class="tech-stack">
        <img src="https://cdn.simpleicons.org/unity/000000" title="Unity" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg" title="C#" />
      </div>
    url: "/projects/modular-ai-system/"
    btn_label: "Learn More"
    btn_class: "btn--primary"

# PROJECT 2
project_AmorExMachina:
  - image_path: /assets/images/AmorExMachinaLogo.png
    alt: "Amor Ex Machina"
    title: "Amor Ex Machina"
    excerpt: |
      Amor Ex Machina is a 3D stealth/puzzle game for PC in which you play as Gabriel, a robot with thoughts and emotions. Sneak, disable, and take over guards to make your way through a robot facility to save Gabriel's kidnapped partner. <br />
      Amor Ex Machina is a vertical slice project done over the course of eight weeks by seven game design students studying at Uppsala University. <br />
      <br><br>
      <div class="tech-stack">
        <img src="https://cdn.simpleicons.org/unity/000000" title="Unity" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg" title="C#" />
      </div>
    url: "/projects/combat-prototype/"
    btn_label: "Learn More"
    btn_class: "btn--primary"

    # PROJECT 3
project_CastByLight:
  - image_path: /assets/images/CastByLightLogo.jpg
    alt: "Cast By Light"
    title: "Cast By Light"
    excerpt: |
      Control the light, to find your light. Cast By Light is a 2D single player puzzle game created for arcade and mobile. The player controls the sun with a rotating dial, creating shadows in the game to solve environmental puzzles to help the protagonist of the game Ann to find her lost partner in a grueling world where the sun is dangerous and the only way is to navigate through the shadows.<br />
      <br><br>
      <div class="tech-stack">
        <img src="https://cdn.simpleicons.org/unity/000000" title="Unity" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg" title="C#" />
      </div>
    url: "/projects/combat-prototype/"
    btn_label: "Learn More"
    btn_class: "btn--primary"

    
---

<style>
  /* --- 1. RESET PAGE PADDING --- */
  
  .page__content {
    padding-top: 0 !important;
  }

  /* --- 2. BIO SECTION (THE BLACK BOX) --- */
  .bio-wrapper {
    background-color: #121212;
    color: white !important;
    
    /* CONTROL THE HEIGHT HERE */
    padding-top: 50px;
    padding-bottom: 0px;
    
    /* Add a clean grey line at the bottom of the black box */
    border-bottom: 1px solid #333; 
    
    /* BREAKOUT LOGIC: Makes it full width */
    width: 100vw;
    position: relative;
    left: 50%;
    right: 50%;
    margin-left: -50vw;
    margin-right: -50vw;
    margin-top: 0; 
  }

  /* --- 3. INNER CONTENT CONSTRAINT --- */
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
  
  /* Stops the internal row from pushing the bottom out */
  .bio-wrapper .feature__row {
      margin-bottom: 0 !important;
      border-bottom: none !important; /* Removes any double lines */
  }

  .page__footer-follow a[href*="feed"],
  .page__footer-follow a[href*=".xml"],
  .fa-rss-square {
    display: none !important;
  }
  .page__footer-copyright {
    display: none !important;
  }
</style>

<div class="bio-wrapper">
  {% include feature_row id="introduction" type="left" %}
</div>

<div id="projects" class="container">
  <h2 style="text-align: center; margin-top: 50px;">School Group Projects</h2>
  
  {% include feature_row id="project_Gracebound" type="left" %}
  <hr>
  {% include feature_row id="project_AmorExMachina" type="right" %}
   <hr>
  {% include feature_row id="project_CastByLight" type="left" %}
</div>


