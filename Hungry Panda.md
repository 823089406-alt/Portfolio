<img width="2830" height="1774" alt="image" src="https://github.com/user-attachments/assets/29edd8e1-6f48-47f1-aa68-2f881129d644" /># Sprint 1 Documentation

**Project Title -** Hungry Panda
---

## Overview & Project Description

"Hungry Panda" is a pixel-style platformer filled with adventure and reflection. Players take on the role of a kung fu-skilled panda, challenging themselves across four unique worlds, avoiding enemies, collecting bamboo, and uncovering the story behind each level. The game blends humor and critique, using level design to encourage players to reflect on deeper themes while enjoying a fun and engaging experience.

---
## Core Gameplay

The core gameplay of our game involves players using an Arduino controller to evade obstacles and traps while collecting bamboo energy along the way to save the panda’s homeland. The game consists of four stages, with difficulty increasing as the levels progress. In the first stage, the panda must avoid demons, traps, and gears to reach the finish line. Then, it progresses to the second stage, and so on, until finally reaching the last stage and achieving victory.

<img width="3278" height="1226" alt="image" src="https://github.com/user-attachments/assets/29be6f91-3850-4f28-a8b1-60b465938438" />

---
## Game Structure & Final Images 
**Game Structure**
 
<img width="3256" height="1476" alt="image" src="https://github.com/user-attachments/assets/6995ea27-6171-4f5e-bf42-362a65be952a" />


**Final Images**

<img width="3186" height="2012" alt="image" src="https://github.com/user-attachments/assets/f37fe547-015d-46f8-a0cb-753f6f5b83b8" />

<img width="2482" height="792" alt="image" src="https://github.com/user-attachments/assets/c3229b5c-70c7-4c5a-bc73-a7a911baabbb" />

---
## 控制器展示

---

## Work Distribution
---

## Supplies & Materials

### Components Used:

- **Material:** Newspaper, Napkin, White latex glue, Electrical wire, Conductive beads, Conductive circular sheets, Conductive tape  
- **Arduino Board:** Arduino Leonardo  
- **Input Components:**  Conductive beads  
- **Output Components:** 
  
### Software Used: 
- **Software:** Unity, Procreate, Midjouney, ChatGPT

---

## Process
### 1.Our first step was brainstorming, during which we initially established three key elements:

* Defining the game's visual style and gathering reference images.
  
<img width="2900" height="574" alt="image" src="https://github.com/user-attachments/assets/31e5730e-375f-4ea5-86f7-3263622fe6a3" />

* Researching similar games and simulating level design elements.

<img width="2350" height="1896" alt="image" src="https://github.com/user-attachments/assets/b8fba464-eece-478f-ab10-d86f49a86430" />

* Developing the background story for the main character.

<img width="2350" height="1896" alt="image" src="https://github.com/user-attachments/assets/f8f18efe-a94b-41e2-920c-526998183022" />

### 2.In the second step, we worked on level design.
* First, we used MidJourney to generate our background images.

<img width="2250" height="990" alt="image" src="https://github.com/user-attachments/assets/a12acd1e-a9ae-4ad2-899f-5194470dc9ff" />

  
* Then, we sourced free pixel-style assets from the Unity Asset Store to create our terrain.

<img width="3104" height="656" alt="image" src="https://github.com/user-attachments/assets/8b411bef-b504-46e2-9510-26092dcf9ace" />

  
* We finalized the design of our character, including animations, and also created animations for monsters and treasure chests.
  
<img width="2732" height="1968" alt="image" src="https://github.com/user-attachments/assets/75703a24-0aef-4fad-bfc2-1a421dce8d97" />
<img width="3268" height="1568" alt="image" src="https://github.com/user-attachments/assets/acf73621-872b-42d1-a000-dacb4b6dd948" />


* Finally, we completed the level design. In the level design process, I first created the basic terrain and added colliders to it. Then, I incorporated **traps** such as saws, spikes, and monsters. Next, I added **a bulletin board** to provide simple hints for the game. I also designed **two possible paths**, with one underground route leading to a dead end. Finally, I implemented a **checkpoint** system—when the character reaches a checkpoint, they will progress to the next level.

<img width="2126" height="2008" alt="image" src="https://github.com/user-attachments/assets/97964472-7a3f-430b-912a-8fc258792064" />
<img width="3132" height="1138" alt="image" src="https://github.com/user-attachments/assets/50a8eb35-b922-47af-bfda-ad24b30d79cc" />

### 3.We completed the full coding implementation for the character and all necessary game objects.

* First, based on the level design, we determined all the necessary actions and settings for the Player. We then decided to split the Player's script into **PlayerLife and PlayerMovement**.
>
>**Player Life** is responsible for implementing the player's death mechanism. When the player collides with an object tagged as "Trap" (such as a trap), the character will trigger the death animation and play the death sound effect.
>
<img width="3268" height="1568" alt="image" src="https://github.com/user-attachments/assets/a0dd4c62-f782-4a19-a4fc-37d24c7befde" />


>
>**Player Movement** is primarily responsible for handling the player's movement and jumping controls, supporting both keyboard input and UI button (touchscreen) controls. In this script, we have implemented:
>
<img width="3132" height="1138" alt="image" src="https://github.com/user-attachments/assets/0e22e42e-9f41-4030-9c51-98150aaf83fa" />


## Video Demonstration
https://youtu.be/dGJplNLhig8



---

**1. Project Goal**

Hungry Panda is a 2D platformer game with motion-based controls. Players use a physical pressure sensor to control the character’s movement, jumping, and attacking. The goal is to eat all the food, avoid enemies, and reach the end of the level!

**2. Current Progress**

We completed the following:

* Basic character actions (movement, jumping, attacking)

* Camera follow optimization

* Basic enemy AI

* Scene loading & level transitions

* Input mapping for the physical pressure sensor

**3. Gameplay Optimization**

* Smoother character controls: Movement currently feels a bit stiff, so we plan to adjust the Rigidbody speed curve and possibly add interpolation.

* Smarter camera movement: We can use Unity’s Cinemachine for smoother camera tracking.

* Improved enemy AI: Right now, enemy movement is too rigid. Next, we plan to implement a state machine so enemies can react dynamically based on the player's position.

**4. Adaptive difficulty:**

* If a player gets stuck for too long, we will slow down enemies or provide hints.

* If a player progresses too quickly, we will add obstacles or increase enemy AI difficulty.

**5. Next Sprint Plan**

✅ Enhance level design: Add varied terrain, traps, and hidden areas.

✅ Improve interactions: For example, eating special food can temporarily speed up or enlarge the character.

✅ UI optimization: Make the HUD more visually appealing, possibly adding animation effects.

✅ Refine sensor experience: Ensure smoother input and reduce accidental triggers.





