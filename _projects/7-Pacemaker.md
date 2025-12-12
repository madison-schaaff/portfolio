---
layout: project
title: MAE 3260 Pacemaker Control Systems Modeling
description: Closed-Loop System Modeling, Control Design, and MATLAB Analysis
technologies: [MATLAB, Laplace Transform Methods, Control Systems]
image: /assets/images/pacemaker.jpg
---

### Project Overview
For my MAE 3260 Final Group Work project, I helped model and analyze a **closed-loop pacemaker–heart system** using tools from system dynamics and control theory. The goal of this project was to design a controller capable of regulating heart pressure output in the presence of disturbances, ensuring a stable and healthy pacing response.  

A pacemaker can be viewed as a real-time feedback system: it senses electrical activity from the heart, processes that information through control logic, and delivers corrective impulses when needed. Our model captures this behavior through block diagrams, transfer functions, Laplace-domain analysis, and MATLAB simulations. Through this work, we evaluated PD, PI, and PID controllers to determine which was best suited for maintaining a stable heart rhythm.

---

### System Modeling & Block Diagram Development
To model the pacemaker, we first defined the heart as a **dynamic system** in which input voltage produces a pressure output. We assumed a linear relationship between the two based on literature models :contentReference[oaicite:0]{index=0}.  

We explored two possible modeling structures:

1. **A full disturbance-driven model**, using reference heartbeat inputs, blood-flow dynamics, and voltage disturbances  
2. **A simplified pacemaker control model**, where the reference input is zero and disturbances are modeled as impulses  

The second approach provided clearer analytical results and aligned more directly with controller design goals. The resulting block diagram captures:

- The pacemaker controller  
- The heart’s transfer function  
- Voltage disturbance inputs  
- Pressure output  
- Error dynamics  

<p align="center">
  <img src="https://github.com/madison-schaaff/portfolio/raw/main/assets/images/block.jpg"
       alt="Pacemaker–Heart Block Diagram"
       width="450"/><br>
  <em><strong>Figure 1.</strong> Pacemaker–Heart Block Diagram</em>
</p>


---

### Transfer Function Derivations & Controller Analysis
Once the block diagram was finalized, we derived the Laplace-domain transfer functions for the system:

- The relationship between disturbance input and pressure output  
- Error expressions for **PD**, **PI**, and **PID** controllers  
- Steady-state behavior using the **Final Value Theorem**  

We computed closed-loop error equations for all three controllers. Through symbolic manipulation and hand calculations, supported by MATLAB, we evaluated how each controller handled disturbances.

<p align="center">
  <img src="https://github.com/madison-schaaff/portfolio/raw/main/assets/images/FVT.jpg"
       alt="Transfer Function and Controller Error Calculations using Final Value Theorem"
       width="700"/><br>
  <em><strong>Figure 2.</strong> Transfer Function and Controller Error Calculations using Final Value Theorem</em>
</p>


---

### MATLAB Simulation & Validation
To validate our analytical results, we wrote MATLAB scripts that plotted error vs. time for each controller.  

The simulations confirmed the core findings derived from the Final Value Theorem:

- **PD controller** → non-zero steady-state error  
- **PI controller** → zero steady-state error  
- **PID controller** → zero steady-state error, but more noise-sensitive due to derivative action  

Given the biological complexity of heart signals, derivative terms can amplify noise and cause instability, making PI control the most practical and robust choice.

<p align="center">
  <img src="https://github.com/madison-schaaff/portfolio/raw/main/assets/images/error.jpg"
       alt="Error Response for PD, PI, and PID Controllers"
       width="450"/><br>
  <em><strong>Figure 3.</strong> Error Response for PD, PI, and PID Controllers</em>
</p>


---

### Results & Controller Selection
From our analytical and computational results, we concluded:

- A **PI controller is the optimal choice** for a pacemaker system.  
- It eliminates steady-state error without the noise sensitivity introduced by derivative action.  
- It provides smooth tracking of desired heart behavior and effectively rejects electrical disturbances.  
- The simplified controller also aligns well with pacemaker hardware constraints, which prioritize reliability and low power consumption.

---

### Additional Exploration: Step Input Analysis
We also explored how the system would behave if the pacemaker responded to a **step reference input**, representing conditions where the heart rate changes abruptly. Using an integral controller, we again found that steady-state error was eliminated, reinforcing the importance of integral action in cardiac control devices.

---

### My Contribution
Although this was a collaborative project, my individual contributions included:

- Analyzing how P, PI, and PID controllers differently affect system error and response behavior  
- Applying Laplace transforms and Final Value Theorem to derive steady-state errors  
- Helping compare controller performance in the context of cardiac pacing  
- Contributing to the overall interpretation of results and selection of the most appropriate controller  

Through this work, I gained insight into how control theory is applied to real biomedical systems, and how controller structure impacts stability, accuracy, and robustness in life-critical devices.

---

### Summary
This project demonstrated the power of feedback control in biomedical engineering applications. By modeling the heart-pacemaker system, generating block diagrams, deriving analytical transfer functions, and validating results through MATLAB simulation, we identified the PI controller as the optimal solution for stable cardiac pacing.  

This experience strengthened my understanding of:

- Closed-loop system behavior  
- Controller design and selection  
- Laplace-domain analysis and steady-state error evaluation  
- Real-world tradeoffs between stability, noise rejection, and simplicity  

It also deepened my interest in applying control engineering to safety-critical systems.
