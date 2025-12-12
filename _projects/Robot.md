---
layout: project
title: MAE 3780 Autonomous Robot – Final Mechatronics Project
description: Mechanical Design, Prototyping, CAD, and Mechatronic Integration
technologies: [Arduino, SolidWorks, Fusion360]
image: /assets/images/robotcad.jpg
---

### Project Overview
For my MAE 3780 final project, I helped design, fabricate, and integrate an autonomous robot capable of navigating a color-coded arena, avoiding boundary lines, and collecting foam blocks for points. The robot combined **mechanical design**, **embedded motor control**, and **sensor-based navigation** under strict size and budget constraints.

Our final robot used:
- Two QTI reflectance sensors for border detection  
- Dual H-bridges powering differential-drive DC motors  
- An Arduino for all logic and timing  
- A passive, mechanically optimized acrylic collection system  

The robot performed reliably during competition—winning **4 of 5 round-robin matches** and advancing to the top 16. It consistently detected board boundaries, executed sweeping behaviors, and collected blocks through its mechanically robust design.

**Figure 1. Final Competition Robot**  
![robot](https://github.com/madison-schaaff/portfolio/raw/main/assets/images/robot.jpg)

---

### Mechanical Design & My Contribution
I was responsible for **all mechanical engineering aspects of the robot**, including ideation, prototyping, CAD modeling, material selection, fabrication, and integration with the electrical system.

#### My mechanical contributions included:
- **Early prototyping** with cardboard and foam to test collection concepts  
- Creating all **CAD models** for the robot body, walls, brackets, and fitment constraints  
- Designing a **rigid three-sided passive collection box** that maximized block capture while fitting within the 8" × 8" size limit  
- **Integrating the structure** with motors, H-bridges, wiring, and the Arduino without interfering with sensors or mobility  
- Ensuring proper **clearance, mass distribution, and structural reinforcement** to withstand collisions  
- Assembling and securing all mechanical components during the final build  

The mechanical system was designed to be:
- **Heavy enough** for stability in collisions  
- **Simple enough** to avoid failure modes  
- **Stiff enough** to maintain geometry during impacts  
- **Open enough** for quick access to wiring and debugging  

This approach reduced complexity, improved reliability, and allowed the team to focus on refining the control logic.

**Figure 2. CAD Model of Final Robot**  
![robotcad](https://github.com/madison-schaaff/portfolio/raw/main/assets/images/robotcad.jpg)

---

### Control Strategy & Robot Behavior
Although I did not write the full control code, I integrated all mechanical components to ensure the sensing and electronics could function properly. The team implemented a QTI-based navigation strategy that my mechanical layout fully supported.

The robot followed this logic:
- **Move forward** when both QTI sensors read white  
- **Rotate 45° left or right** when only one sensor detects black  
- **Perform a 180° turn** when both sensors detect black  
- **Execute a timed 90° turn** at the halfway mark to begin sweeping blocks  
- **Stop automatically** after ~60 seconds  

This behavior enabled consistent border detection and predictable sweeping motion.

**Figure 3. Strategy Flowchart**  
![flowchart](https://github.com/madison-schaaff/portfolio/raw/main/assets/images/flowchart.jpg)

---

### Iterative Design Process
Our project evolved over several milestones, influenced heavily by mechanical feasibility and integration challenges.

#### Initial concept — active arm-based collection  
I prototyped a motor-driven arm system to scoop blocks, but integrating additional motors with the sensors caused:
- Interference with QTI placement  
- Wiring congestion  
- Balance and stability problems  
- Increased budget and complexity  

#### Final concept — passive collection box  
After validating prototypes, I redesigned the mechanical system around a **passive acrylic box**, which:
- Required no moving parts  
- Was lighter, more reliable, and easier to assemble  
- Added structural rigidity to handle collisions  
- Provided consistent block collection performance  
- Freed space for clean sensor mounting and wiring  

This mechanical simplification directly improved the reliability of the robot’s navigation logic.

---

### Competition Performance
Despite minor turning inconsistencies, our robot performed strongly:
- **Advanced to the top 16**  
- Won **4 out of 5** round-robin matches  
- Maintained good stability due to its weight and structural design  
- Successfully detected borders and swept blocks into the collection box  

Some blocks escaped during tight turns due to the open front section—an issue that could be resolved with a mechanical gate or hinged flap.

---

### Lessons Learned & Future Improvements
From a mechanical perspective, key improvements for future versions include:
- Adding a **front cover or gate** to prevent block loss during turns  
- Increasing weight strategically to boost pushing power  
- Mounting an **additional QTI sensor at the rear** for more accurate boundary detection  
- Using reinforced materials or multi-layer acrylic for higher rigidity  
- Designing a more modular structure for faster debugging of electrical systems  

This project strengthened my experience in:
- Mechanical design for mechatronic systems  
- Rapid prototyping and iterative physical testing  
- Sensor and wiring integration within tight geometric constraints  
- Collaborating across mechanical & embedded software roles  

---

### Summary
I served as the **mechanical engineer** for this autonomous robot project—leading the prototyping, CAD, fabrication, structural design, and hardware integration. The final robot demonstrated strong performance, stability, and reliability, showcasing a balance between mechanical simplicity and functional effectiveness.

This project developed my skills in mechatronics integration, mechanical CAD, design-for-assembly, and system-level engineering, preparing me for future robotics and embedded systems work.

