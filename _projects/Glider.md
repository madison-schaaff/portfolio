---
layout: project
title: MAE 3050 Hand-Launched Glider – Final Design Project
description: Aerodynamics, Flight Mechanics, Prototyping
technologies: [SolidWorks, MATLAB, Flight Testing]
image: /assets/images/glidercad.png
---

### Project Overview
For my MAE 3050 Final Design Report, I helped design, build, and test a hand-launched glider intended to maximize **time aloft** over a flight distance of ~15 meters. The design work modeled a real-world engineering challenge inspired by the Tarrytown Mission—an atmospheric sampling scenario in which a glider must remain airborne as long as possible while carrying a payload.  

The project required balancing **aerodynamics, structural considerations, manufacturability, and stability**, under constraints such as:
- Maximum wingspan of 6 m (scaled-model equivalent)  
- Total mass under 25 kg (scaled-model equivalent)  
- 10 kg payload requirement (scaled)  
- Operation in the **incompressible** flow regime  

After initial prototypes underperformed, I helped lead the redesign effort, incorporating a **dihedral elliptical wing**, improved sanding and shaping, and mass distribution adjustments to achieve a more stable and longer-duration glide.

---

### Tarrytown Glider Design
Our Tarrytown Glider (TG) was developed first, using the atmospheric properties of Tarrytown and ideal aerodynamic relationships to determine optimal wing geometry, aspect ratio, and operating velocity.

Key aerodynamic choices included:
- **Elliptical wing planform** for minimized induced drag  
- **Dihedral wing configuration** to improve roll stability  
- **Thin, streamlined fuselage** to minimize drag  
- **Maximized wingspan** within constraints to improve lift  

We selected an aspect ratio near **AR = 6.0**, balancing structural integrity with induced drag reduction. Using incompressible aerodynamic models, we calculated:
- Chord length  
- Wingspan  
- Planform area  
- Lift and drag coefficients  
- Mach number (< 0.3 requirement)  
- Reynolds number (~23,000), confirming incompressible conditions  

These calculations guided all geometric and performance decisions.
---

### Earth Glider (Scaled Prototype)
To test the design physically, we constructed an Earth Glider (EG) scaled by a factor of **9.32:1** relative to the TG. Our goal was to maintain:
- The same **aspect ratio (6.045)**  
- Nearly identical aerodynamic behavior  
- Similar Reynolds number  
- Corresponding lift and drag coefficients  

Scaling calculations determined EG values for:
- Chord length  
- Wingspan  
- Stabilizer areas  
- Fuselage length  
- Flight speed & stall speed  

We fabricated the EG from balsa wood, sanding the wings to produce an elliptical shape and smooth airflow. Control surfaces (ailerons, elevator, rudder) were built using taped additions, which allowed for iterative adjustments during testing.

**Figure 1. Glider Final Design**  
![glider](/assets/images/glider.jpg)

**Figure 2. Glider Final Design CAD**  
![glidercad](/assets/images/glidercad.jpg)

---

### Flight Testing & Results
The Earth Glider was hand-launched over a 15-meter range. From calculations, we predicted:
- **Flight speed:** 3.35 m/s  
- **Time aloft:** 4.48 s  

Actual testing produced:
- **Flight speed:** ~5 m/s  
- **Time aloft:** ~3 s  

Although faster than predicted (reducing time aloft), the EG demonstrated:
- Stable roll behavior in most trials  
- Ability to consistently cross the finish line  
- Effective lift generation for its scale  

A key observation was that hand-launch variability caused significant deviation from theoretical performance. Launch speed and pitch angle influenced the flight path more than expected.

Control-surface issues also contributed to rolling during some trials—tape flexed under airflow and even during the throw. Future designs should reinforce these with multilayer tape or lightweight rigid materials.

---

### Engineering Analysis & Insights
Through calculations and testing, we measured how well the EG approximated the TG. Several ratios (wingspan, chord, Reynolds number) aligned well, confirming accurate geometric scaling. However, Mach number differences and real-world launch variability reduced the predictive fidelity of the EG.

By analyzing performance metrics such as glide ratio, sink rate, static margin, and lift/drag forces, we learned:
- The EG is a **reasonable but imperfect predictor** of TG behavior.  
- Matching Reynolds number alone is insufficient when Mach numbers differ significantly.  
- Static margin adjustments require precise mass placement—added clay increases weight and reduces flight time.  
- Structural modifications (lighter stabilizers, thinner wings) could improve performance in future iterations.

---

### My Contribution
Across design, engineering, and testing, I contributed to:

- Aerodynamic sizing calculations for chord, wingspan, aspect ratio, and Reynolds number  
- Identifying necessary redesign changes after the initial prototype failed  
- Constructing and sanding the elliptical dihedral wings  
- Adjusting control surfaces and center-of-gravity placement to improve stability  
- Assisting with theoretical glide and flight-time predictions  
- Supporting the final analysis comparing TG and EG performance  

This project strengthened my understanding of **aerodynamics, scaling laws, flight mechanics, and iterative physical prototyping**, and demonstrated how theoretical performance models translate into real-world behavior.

---

### Summary
This glider project integrated concepts from fluid mechanics, aerodynamics, dynamics, and hands-on prototyping. By designing both a theoretical Tarrytown Glider and a scaled Earth Glider, I gained experience in:
- Aerodynamic optimization  
- Flight stability design  
- Scaling and similarity principles  
- Physical fabrication and testing  
- Performance evaluation under real-world conditions  

The work reflects a complete engineering cycle—from modeling to physical testing—and challenged me to reconcile idealized calculations with real aerodynamic behavior.

