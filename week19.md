# Final Project Portfolio

## Project Details and Links

- **Name**：Yu Chen
- **Group Members**：Xue Dong; Yiwen Chen; Yifei Guo
- **Project Title**：Shadow and Shard

---

## Project Overview
**Shadow and Shard** is an interactive art experiment built upon a Unity + Arduino + AI toolchain. Inspired by four historical artworks, this project transforms viewers into **operators and restorers**, inviting them into a game world of fragments, shadows, and memory through **physical touch, virtual reconstruction, and procedural feedback**.
In this museum, exhibitions no longer remain static, and artifacts are no longer just gazed upon — they are manipulated, activated, and reassembled.

Our central question is:
>When the game becomes the medium of viewing, does art still retain its ambiguity and silence?
>When AI-generated imagery replaces manual reproduction, are we witnessing a reconfiguration of artistic authority?

---

## Inspiration and Research Background
The core premise of Shadow and Shard is:

**How can we invite audience participation without dissolving the aura of art?**

Grounded in the logic of interactive museums, and drawing on contemporary game design and generative AI tools, we explore the blurred boundaries between art, technology, and spectatorship.'

### **The Logic of Viewing in Museums: From Gaze to Participation**

Our inspiration began with a critique of traditional museum experiences — where viewing is static, authoritative, and non-interactive. The museum establishes a boundary between viewer and object (Hooper-Greenhill, 2000). Yet, as digital media enters the space, this boundary begins to shift.

As Claire Bishop notes, “Contemporary art increasingly aims to produce participation, not just presentation.” (Bishop, Artificial Hells, 2012)
In this spirit, we introduced **participatory aesthetics** into our project — allowing players to “enter” the artwork via touch sensors, fragment collection, and interactive reassembly.
<img width="1928" height="580" alt="image" src="https://github.com/user-attachments/assets/fe5fccd1-7753-4bdf-b785-b49cbde7f410" />


### **AI-Generated Reproduction**

We relied heavily on tools like Midjourney and Tripo AI for visual and spatial design. Due to time constraints, we needed to rapidly create backgrounds and UI elements — but this raised a critical concern:

**Does AI-assisted creation undermine creative ethics?**

As Lev Manovich observed, “AI-generated images are cultural shortcuts — and ethical blind spots.” (Manovich, 2020)
But in our view, these images do not appear out of nowhere — they are trained on the fragments of history. In that sense, we are using fragments of the past to generate new visual fragments of our own.

### **Game Mechanics as Cultural Language**

Mechanics like **levels, collection, and timed challenges** are not just tools of game design — they carry implicit cultural values: efficiency, control, and feedback addiction.

As McKenzie Wark writes in Gamer Theory (2007):

>“Games are idealized control systems. They offer the illusion of freedom within a highly structured world.”
We use these game systems to guide players in “restoring art” — while simultaneously questioning whether that guidance is itself a form of control.

---

## Game Flow Design
In our interactive museum experience, users begin by entering the exhibition space and observing various 3D-printed art replicas. By touching a selected replica, an Arduino sensor detects the interaction and triggers the corresponding game level in Unity. Players then use a custom Arduino controller to navigate challenges such as jumping and collecting "art fragments" 🧩. Once all fragments are collected, the game unlocks an audio narration revealing the story behind the artwork. After completing a level, users return to the main selection interface and can continue exploring other artworks.

<img width="1752" height="946" alt="image" src="https://github.com/user-attachments/assets/bf6a8ca3-e58a-4e3b-8676-8207bb8d05dd" />


---

## Four Levels of Shadow and Shard
We designed four game levels based on culturally symbolic artworks. Each level combines **interaction mechanics, artistic imagery, and critical narrative**. By touching real-world 3D-printed replicas of artifacts, players enter each level and engage in fragment collection and reinterpretation within a digital space.

### **Level 1｜A Thousand Miles of Ink**
 
This level integrates the visual language of classical Chinese landscape painting with rhythmic gameplay mechanics. It transforms a traditional ink scroll into an immersive rhythm game where touch replaces keyboard input.

- **Artwork Inspiration**：*A Thousand Li of Rivers and Mountains*, Wang Ximeng, Northern Song Dynasty
- **3D-Printed Object**：High-resolution mountain terrain segments
- **Game Mechanic**：Players control four directions via MPR121 touch sensors. As notes fall into the timing zone, the player taps precisely to receive “Perfect”, “Good”, “Normal”, or “Miss” ratings. The level includes combo multipliers and a real-time score feedback system for synchronized audiovisual engagement.

**Technology & Interaction**

- **Arduino**：Touch sensors embedded in the printed mountain landscape;
- **Unity**：Manages rhythm timing, note generation, hit judgment, and final score display.

<img width="2032" height="502" alt="image" src="https://github.com/user-attachments/assets/3223f1b0-270f-43b7-9d34-0dffbb6deb3c" />

---

**Level 2｜Stairs of Victory**

This level draws from the symbolism of Nike, the Greek goddess of victory, and reimagines it with a “whack-a-mole”-style mechanic where players collect coins via interactive sculpture.

- **Artwork Inspiration**：*Nike of Samothrace* (Louvre Museum, Greece)
- **3D-Printed Object**：Upper torso of the Winged Victory statue
- **Game Mechanic**：Players collect appearing golden coins. Missing coins deduct 1 health point (3 total). Collect enough before running out of lives to win the level.

**Technology & Interaction**

- **Arduino**：Touching the statue starts the game. MPR121 sensors (installed on the lotus leaves) allow the player to control movement (forward, back, jump);
- **Unity**：Randomized coin generation and real-time collection.

<img width="1988" height="688" alt="image" src="https://github.com/user-attachments/assets/5eb040c0-75c2-4586-a61d-ca5ac6d392d8" />

---

**Level 3｜Heart of the Water Lilies**

Inspired by Impressionism’s fascination with ephemeral light, this level is a sensory challenge about time, flow, and perception. Players step into a dreamy water-lily lake, collecting glowing fragments before the light fades.

- **Artwork Inspiration**：*Water Lilies*, Claude Monet (France)
- **3D-Printed Object**：Floating lily model
- **Game Mechanic**：Timed challenge with speed-up/slow-down elements

**Technology & Interaction**

- **Arduino**：Touching the lily model activates the timer;The player controls movement and jumping using three flower petals to navigate through the level.
- **Unity**：The player auto-moves forward, dodging “bubble” traps and collecting “light butterflies” for speed boosts. Fragment positions are randomized. Time limit: 2 minutes.

<img width="3090" height="672" alt="image" src="https://github.com/user-attachments/assets/94473155-f794-4c1e-963a-37b491402dc3" />


---

**Level 4｜Porcelain Labyrinth**

This level reinterprets the elegance and complexity of Ru ware porcelain into a musical maze experience, where rhythm and spatial navigation converge.

- **Artwork Inspiration**：*Ru Ware Dragon Relief Vase*, Song Dynasty, China
- **3D-Printed Object**：Complete Ru-style celadon vase
- **Game Mechanic**：Rhythm-based clicking (similar to music reaction games)

***Technology & Interaction**

- **Arduino**：Touching the landscape replica triggers entry into the maze;
- **Unity**：2D maze navigation, collect all fragments to unlock the closing narration.
  
<img width="2212" height="482" alt="image" src="https://github.com/user-attachments/assets/3857d360-155a-4085-b786-5db476a26646" />

  
---

## Technical Architecture（Level 2）
In *Shadow and Shard*, Arduino serves not only as the physical trigger to launch the game, but also as a body-based interactive controller that replaces traditional keyboard input. The system consists of two main hardware interaction modules, working in coordination with Unity and AI tools to form a complete human-computer interaction loop.

### Arduino Interaction Module

|---------------|:---------------------------------------------|

**Module 1: Game Start Touch Module**

**Hardware Components:**
- (MPR121)touch sensor + Arduino Uno
- Each touchpoint is linked to a 3D-printed replica of an artifact
<img width="2268" height="922" alt="image" src="https://github.com/user-attachments/assets/782ed39e-d3fd-494c-9d07-5d5a52e470e2" />


**Function Description:**
- Each artwork is assigned a unique ID;
- When touched, the Arduino detects the ID and sends it to Unity via serial communication;
- Unity receives the ID and loads the corresponding game level.
<img width="1870" height="778" alt="image" src="https://github.com/user-attachments/assets/abd29d8f-c6be-43ef-9101-ea66e18819b5" />

**Module 2: Arduino Controller System (MPR121-Based Directional Input)**

In Level 2: The Heart of Water Lilies, we aimed to replace traditional keyboard input with bodily touch interaction, allowing players to control the character using physical gestures. This interaction is achieved through the Adafruit MPR121 capacitive touch sensor in combination with an Arduino microcontroller.

**1. Hardware Components**
- MPR121 capacitive touch chip
- Custom conductive input panel, made from copper tape, conductive fabric, or wire
- Arduino board

**2. Wiring Diagram**

<img width="1682" height="1188" alt="image" src="https://github.com/user-attachments/assets/6f16f64b-422b-43b7-b27e-67798a4fe2f1" />

Each touch point corresponds to a movement direction. The Arduino reads input from MPR121 and sends a character command via serial. A Python script bridges this signal via **UDP** to **Unity**, which handles real-time character control.

| Action    | Command | Touch Point |
|-----------|---------|-------------|
| First Hole   | `1`     | `i = 1`     |
| Second Hole  | `2`     | `i = 2`     |
| Third Hole      | `3`     | `i = 3`     |
| Fourth Hole     | `4`     | `i = 4` |

**4. Interaction Replacement**

- Replaces keyboard arrow keys to enhance physical engagement;
- Each touch on the MPR121 surface triggers a change in capacitance, which is recognized by the system as a movement input.

  
**5. Advantages**

- Provides greater immersion and a sense of ritual;
- Better aligns with museum-style interactive installations by emphasizing tactile engagement over traditional screen-based control.

### Unity Technical Architecture (Level 2｜Stairs of Victory)
Unity Animation | All Unity Animation can be found here: 

https://git.arts.ac.uk/user-attachments/assets/f2fe705f-1725-43aa-a777-910c22138335

Unity Level2 Secnes | Unity Level2 Secnes can be found here: https://git.arts.ac.uk/24010676/Responsive-Environments-Blog-2024/tree/main/Scenes

Unity Level2 Secnes | Unity Level2 Scripts can be found here:https://git.arts.ac.uk/24010676/Responsive-Environments-Blog-2024/tree/main/Scripts


In this level, Unity handles the full pipeline of visual rendering, gameplay mechanics, and interaction control, while receiving real-time signals from Arduino to support a timed gameplay experience.

<img width="1410" alt="image" src="https://git.arts.ac.uk/user-attachments/assets/25f5ff41-2e1d-474b-9e40-452f050d153b" />




**4. Key Design Highlights**

- Countdown gradually desaturates the visual scene via Post-Processing, enhancing the fading dreamlike aesthetic.
- Touching a butterfly grants a quick Dash, creating a gliding motion effect.
- Touching a bubble deducts 30 seconds and displays a floating damage number.

---
## Art Asset & AI Tools
To create a museum game space that balances artistic richness and immersion, we utilized a blend of AI-assisted tools and custom design workflows to generate environmental assets, UI elements, and spatial moods.

### AI Tools Summary

| Tool Name             | Purpose (EN)                                       | Description (EN)                                           |
|-----------------------|----------------------------------------------------|-------------------------------------------------------------|
| **Midjourney**        | AI image generation for concept art and textures   | *Text-to-image AI for concept art and textures*             |
| **Tripo AI**          | AI-based 3D model generation for sculptures/objects| *AI 3D model generation for statue and object prototyping*  |
| **Photoshop / Illustrator** | Post-processing, icon design, visual refinement | *Image post-processing, UI and icon design*                 |

### Background Generation
![bg](https://git.arts.ac.uk/user-attachments/assets/bb146e71-52e2-4838-b96e-6bc2c405b2ca)



### 3D Generation
![1750377475363](https://git.arts.ac.uk/user-attachments/assets/2545d5ea-2556-4c91-a0b8-241cbe9cf721)


---
## Fabrication Process

To allow the audience to physically “touch art,” we used digital fabrication tools to create four interactive replicas of artworks. These replicas not only visually resemble the original pieces, but also integrate Arduino-based systems to serve as interactive triggers for the game.

### 3D Modeling & Printing
We used Tripo AI to generate 3D models based on reference images of historical artifacts.
The models—such as reliefs, water lilies, and sculptures—were then produced using 3D printers.
<img width="943" alt="image" src="https://git.arts.ac.uk/23009836/Making-3-Final-Project/assets/1322/67051b9b-e796-46b2-9ea6-c31e0a22d7a9">

### Laser-Cut Bases for Hardware
Acrylic or wooden bases were fabricated using a laser cutter.
The bases were designed with wire channels, mounting holes for Arduino boards, and cutouts for power access.
All circuit boards, sensor modules, and USB cables were embedded beneath the base to ensure a clean, stable, and exhibition-ready appearance.
<img width="1041" alt="image" src="https://git.arts.ac.uk/23009836/Making-3-Final-Project/assets/1322/58205b41-bea8-4a89-8920-b6f69acd97f1">

### Arduino Assembly
We implemented a capacitive touch system using Arduino and the MPR121 sensor.
All wires were routed from the 3D-printed replicas into the interior of the base, where the control modules were securely housed.
<img width="919" alt="image" src="https://git.arts.ac.uk/23009836/Making-3-Final-Project/assets/1322/93398a15-98c5-4d2c-b904-30f13d1958d5">


---

## Testing & Iteration

### Touch Sensitivity Adjustment
- In the early phase, copper foil touchpoints frequently caused false or missed touches. We later switched to conductive fabric and lowered the MPR121 sensitivity threshold.
- To prevent repeated unintended actions, we implemented debounce logic on the Arduino side and cooldown mechanisms within Unity.

### Unity Input Latency Optimization
- The initial UDP communication setup had noticeable frame delays. We resolved this by introducing a dedicated background thread for signal listening and handling all command execution in Unity’s main thread, significantly improving response time.
- For “hold-to-move” commands, we added a direction buffer system to ensure smoother and more continuous control.

### Level Pacing Adjustment (Level 3)
- Originally, the level timer was set to 90 seconds, but players reported that this wasn’t enough time to get familiar with the mechanics.
In the updated version, the time limit was extended to 120 seconds. The bubble penalty was increased from 10 to 30 seconds, and fragment positions were randomized to improve replayability.
- We also adjusted the intensity of butterflies (boost effect) and bubbles (slow effect) to maintain better gameplay balance and reduce frustration from disruptive elements.

---

## My Contribution to the Project

### Arduino Integration
I connected and configured the Arduino hardware, programmed sensor input/output, and ensured successful data transmission between Arduino and Unity through serial communication.

### Image Generation
I utilized AI tools to create visual assets, such as backgrounds and characters, to support the visual development of the project.

### Level 2 Unity Scene Development
I was fully responsible for building the Level 2 scene in Unity, including environment design, object placement, event triggers, and interactive logic.

### Start and End Screen Design in Unity
I designed and implemented the start and end screens in Unity, integrating UI elements, transitions, and functionality such as game start, restart, and return to menu.

### Final Documentation Editing
I compiled, organized, and polished all project documentation, including technical explanations, images, and team contributions, ensuring clarity and consistency for final submission.

### PPT Editing
Edited slides for presentation on final presentation day.

---
## Final Project Output
<img width="1285" alt="image" src="https://git.arts.ac.uk/23009836/Making-3-Final-Project/assets/1322/eb723cee-5298-4486-97f7-00259dff417b">
<img width="969" alt="image" src="https://git.arts.ac.uk/23009836/Making-3-Final-Project/assets/1322/720e1f00-e14c-4127-a214-30fe0a4452ac">
<img width="1127" alt="image" src="https://git.arts.ac.uk/23009836/Making-3-Final-Project/assets/1322/9acd440c-1b8b-4053-8e59-eaf58b9eafad">
<img width="1080" alt="image" src="https://git.arts.ac.uk/23009836/Making-3-Final-Project/assets/1322/80f6b683-8016-4853-b220-669ebe6cd163">

---

## Video
https://ual.cloud.panopto.eu/Panopto/Pages/Viewer.aspx?id=376b33d2-589a-4616-9478-b3070170ef18



---
## Design Justification
During the presentation of Shadow & Shard, we received many valuable comments. The visual design, physical interaction, and cultural art integration were well appreciated. The interaction method and interface were seen as creative and engaging.

At the same time, some reviewers suggested explaining the control system more clearly, reducing text on slides, and including more live demos. There were also ideas to simplify the system and reduce the number of Arduino components.

Moving forward, we plan to improve how we present the project, refine the interaction flow, and strengthen the narrative to create a more clear and immersive experience.

![Uploading image.png…]()

