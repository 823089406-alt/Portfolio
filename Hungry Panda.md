# Sprint 1 Documentation

**Project Title -** Hungry Panda
---

## Overview & Project Description

"Hungry Panda" is a pixel-style platformer filled with adventure and reflection. Players take on the role of a kung fu-skilled panda, challenging themselves across four unique worlds, avoiding enemies, collecting bamboo, and uncovering the story behind each level. The game blends humor and critique, using level design to encourage players to reflect on deeper themes while enjoying a fun and engaging experience.

---
## Core Gameplay

The core gameplay of our game involves players using an Arduino controller to evade obstacles and traps while collecting bamboo energy along the way to save the panda’s homeland. The game consists of four stages, with difficulty increasing as the levels progress. In the first stage, the panda must avoid demons, traps, and gears to reach the finish line. Then, it progresses to the second stage, and so on, until finally reaching the last stage and achieving victory.

<img width="1639" alt="image" src="https://git.arts.ac.uk/23009836/Responsive-Environments-Blog-2024/assets/1322/6971ce92-d1d5-46b2-8db3-f09809fd2ccb">

---
## Game Structure & Final Images 
**Game Structure**
 
<img width="1628" alt="image" src="https://git.arts.ac.uk/23009836/Responsive-Environments-Blog-2024/assets/1322/dd9b6e18-619d-477e-b8a3-f2d613fce886">


**Final Images**

<img width="1593" alt="image" src="https://git.arts.ac.uk/23009836/Responsive-Environments-Blog-2024/assets/1322/010a6a33-33ab-48e4-9bf7-22f10d9b53f6">

<img width="1415" alt="image" src="https://git.arts.ac.uk/23009836/Responsive-Environments-Blog-2024/assets/1322/6724dc9a-8d8a-4425-98fa-740bf4731b81">

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
  
  <img width="1241" alt="image" src="https://git.arts.ac.uk/23009836/Responsive-Environments-Blog-2024/assets/1322/48ceb09d-39fb-424a-876b-c702b8ab7f33">

* Researching similar games and simulating level design elements.

  <img width="1450" alt="image" src="https://git.arts.ac.uk/23009836/Responsive-Environments-Blog-2024/assets/1322/68a23890-a9cd-4999-864e-7d176355a9d2">

* Developing the background story for the main character.

  ![image](https://git.arts.ac.uk/23009836/Responsive-Environments-Blog-2024/assets/1322/56fae735-c27e-492d-9987-e1fb45d213df)

### 2.In the second step, we worked on level design.
* First, we used MidJourney to generate our background images.

  <img width="1175" alt="image" src="https://git.arts.ac.uk/23009836/Responsive-Environments-Blog-2024/assets/1322/c4acef01-0693-4e8a-b115-bb4f1c397ffd">

  
* Then, we sourced free pixel-style assets from the Unity Asset Store to create our terrain.

  <img width="1552" alt="image" src="https://git.arts.ac.uk/23009836/Responsive-Environments-Blog-2024/assets/1322/b6f0e26c-b646-4815-9ded-325bb4e713d6">

  
* We finalized the design of our character, including animations, and also created animations for monsters and treasure chests.
  
  <img width="1633" alt="image" src="https://git.arts.ac.uk/23009836/Responsive-Environments-Blog-2024/assets/1322/bd3deabe-edb2-4044-8fc4-8ff4d23e27cc">
  <img width="1366" alt="image" src="https://git.arts.ac.uk/23009836/Responsive-Environments-Blog-2024/assets/1322/8741a963-3f3f-4834-a48b-a2c446511ecb">


* Finally, we completed the level design. In the level design process, I first created the basic terrain and added colliders to it. Then, I incorporated **traps** such as saws, spikes, and monsters. Next, I added **a bulletin board** to provide simple hints for the game. I also designed **two possible paths**, with one underground route leading to a dead end. Finally, I implemented a **checkpoint** system—when the character reaches a checkpoint, they will progress to the next level.

  <img width="1063" alt="image" src="https://git.arts.ac.uk/23009836/Responsive-Environments-Blog-2024/assets/1322/467c0972-3c43-450f-a9e4-8b0e6075debc">
  <img width="1366" alt="image" src="https://git.arts.ac.uk/23009836/Responsive-Environments-Blog-2024/assets/1322/6dcc9260-15cc-4ab0-b093-86ec78973296">

### 3.We completed the full coding implementation for the character and all necessary game objects.

* First, based on the level design, we determined all the necessary actions and settings for the Player. We then decided to split the Player's script into **PlayerLife and PlayerMovement**.
>
>**Player Life** is responsible for implementing the player's death mechanism. When the player collides with an object tagged as "Trap" (such as a trap), the character will trigger the death animation and play the death sound effect.
>
><img width="1634" alt="image" src="https://git.arts.ac.uk/23009836/Responsive-Environments-Blog-2024/assets/1322/b863444f-5de5-45db-b467-8ed28d605a00">

>
>**Player Movement** is primarily responsible for handling the player's movement and jumping controls, supporting both keyboard input and UI button (touchscreen) controls. In this script, we have implemented:
>
><img width="1566" alt="image" src="https://git.arts.ac.uk/23009836/Responsive-Environments-Blog-2024/assets/1322/543de4f6-2f35-4387-a026-9ea66e1c42c0">

* 接着我们编写了物体收集脚本、Camera脚本、Announcement脚本、StickyPlatform脚本、WayPoint脚本、声音脚本。
>物体收集脚本的主要功能是
>

>Camera脚本的主要功能是
>

>Announcement脚本的主要功能是
>

>StickyPlatform脚本的主要功能是
>

>WayPoint脚本的主要功能是
>

>声音脚本的主要功能是
>

* 最后我们完整了整个游戏的控制脚本：开始菜单、结束菜单、全局控制。
>开始菜单脚本的主要功能是
>

>结束菜单脚本的主要功能是
>

>全局控制脚本的主要功能是
>
  
### 4.硬件开发与Arduino代码

* 在硬件开发方面，我们选择了压力传感器，通过将人对传感器的压力来控制Player的跳跃，并取代“空格键”。
>
  
* 在Arduino代码方面，我们在Unity中加入了Arduino相关的脚本，使两者可以结合起来。
>

### 5.物理控制器结构与制作
* 在物理控制器的结构方面，我们依据草图，将整个正方形方框分为上下两个方面。上方用海绵制作而成，同时我们把压力传感器镶嵌在海绵里面，以便于人物可以触摸到传感器。下方我们将连接线和Arduino板与面包板藏进去，使外表看起来更加美观。

* 我们的制作过程主要有四步：
>我首先将废弃的旧纸张剪碎，加入小苏打放到锅中煮烂。

>接着制作一个正方形的架子将其用热熔胶和丝网套牢。

>紧接着将传感器镶嵌进海绵中。

>最终将上下两个空间用热熔胶粘在一起。

>图片

### 6.游戏测试
我们接下来对我们的游戏进行了多方面的测试，其中我们发现了非常多的问题：
* 第一个问题是我们导出Unity文件后，文字出现错位
* 第二个问题是我们四个场景中摄像机的大小不一致
* 第三个问题是，我们设定的从第一关到第四关难度递增，结果我们的难度不相匹配
* 第四个问题是我们的Player移动速度不一致。
* 第五个问题是Player碰撞体与陷阱碰撞体过大。
* 第六个问题是人物站立不到平台上。

### 7.游戏优化升级
最后我们对游戏进行了升级，我们一起来为第三关和第四关增加难度，并且修复了以上问题。

比如，我们让游戏难度逐渐增加。这包括提高怪物的智力和数量，以及增加资源限制。这些变化迫使玩家进行战略思考并快速做出反应，从而创造更激烈、更引人入胜的体验。
图片

## Video Demonstration


---

## Arduino Code


---
## Link to Unity Files


---
## Design Justification 

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




