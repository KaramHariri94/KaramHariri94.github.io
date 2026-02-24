---
title: "Modular AI System"
excerpt: "A decoupled AI architecture using Behavior Trees for the game 'Project Name'."
last_modified_at: 2024-02-24
layout: single
classes: wide
author_profile: true
toc: true             # Creates a "Table of Contents" on the right
toc_label: "Jump to Section"
toc_icon: "list"
header:
  overlay_image: /assets/images/ai-header.jpg # Large splash image at the top
  overlay_filter: 0.5 # Darkens image so text is readable
  caption: "Screenshot: Visual Debugger in action"
sidebar:
  nav: "docs" # Ignore this or delete if not using custom nav
  title: "Project Details"
  text: |
    **Role:** System Architect<br>
    **Engine:** Unreal Engine 5<br>
    **Language:** C++<br>
    **Team Size:** 4<br>
    **Duration:** 3 Months<br>
    
    [<i class="fab fa-github"></i> View Code](https://github.com/KaramHariri94)
---

[< Back to Projects](/#projects){: .btn .btn--light .btn--small}
<br><br>

## 🎯 The Problem
We needed 5 different enemy types that shared core logic (movement, health) but had unique tactical behaviors. 
* **Challenge:** Hard-coding `if/else` chains for every enemy was creating "spaghetti code."
* **Goal:** Create a system where designers could mix-and-match behaviors without asking a programmer.

## ⚙️ The Architecture
I implemented a **Utility AI / Behavior Tree** hybrid system.

### 1. Decoupled Logic
I separated the "Brain" from the "Body."
* **The Body (Actor Component):** Handles physics, animations, and navmesh movement.
* **The Brain (Controller):** Only sends commands like `MoveTo()` or `Attack()`.

```cpp
// Example: The Brain sending a command to the Body
void AEnemyAIController::ExecuteAttack()
{
    if (Blackboard->GetValueAsObject("TargetActor"))
    {
        CombatComponent->RequestAttack(CurrentWeapon);
    }
}