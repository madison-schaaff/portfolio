---
layout: project
title: MAE 2250 CAD Creative Project
description: Advanced Solid Modeling & Feature-Based Design
technologies: [Autodesk Fusion 360]
image: /assets/images/perfume2.jpg
---

### Project Overview
For my MAE 2250 CAD Creative project, I chose to model a **high-end perfume bottle** because it combined geometric complexity, aesthetic detail, and multiple internal components that challenged my existing CAD skillset. The project required replicating the external glass housing, internal pump mechanism, nozzle, and label features with attention to both form and function.  

My goal was to create a fully parametric, assembly-ready model that accurately represented the real product while demonstrating advanced CAD features such as chamfers, fillets, text embossing/debossing, multi-body workflows, and proper joint definitions.

---

### Modeling Strategy
I began by studying the physical bottle and creating **dimensioned hand sketches** of the main geometry, focusing on the rectangular base, angled top, interior cavity, label recess, and pump mechanism. After capturing major dimensions, I developed a structured modeling plan:

1. **Model the bottle body first**, beginning with a rectangular prism to establish the primary form.
2. **Add complex transitional geometry** using chamfers and fillets to replicate the angled, smooth surfaces around the nozzle region.
3. **Carve out the internal glass cavity** using offset planes and cut operations to create realistic wall thickness.
4. **Model internal components separately**—the tube, nozzle, and pump—because they required detailed topology that was easier to control in isolated part files.
5. **Assemble all components** using rigid joints to match how the real bottle behaves (no degrees of freedom between parts).

This modular workflow allowed me to refine each component efficiently before integrating them into a complete assembly.

---

### Key Modeling Decisions
- **Chamfer–Fillet Combination for the Bottle Top:**  
  The real perfume bottle transitions from sharp edges to a smooth, angled slope. After experimenting with arcs, sweeps, and surface blends, I found that a **multi-distance chamfer followed by selective filleting** produced the most accurate geometry.

- **Emboss/Deboss for Text and Patterning:**  
  I used **deboss** to engrave the front label area and the top of the pump, and **emboss** for the bottom glass pattern, which consisted of repeated text characters forming a geometric texture.

- **Material Assignments:**  
  - Bottle: Pink-tinted glass  
  - Pump/Nozzle: Stainless steel  
  - Label text: Painted black  
  - Tube: White plastic  

  Assigning accurate materials was essential for producing realistic renderings.

- **Separate Part Modeling for the Pump Assembly:**  
  The pump required a **nested cylindrical shell, rotating nozzle, and tube**, so I used a top-down approach to ensure proper fit between components. The nozzle was connected via a revolute joint to allow realistic motion in renders.

---

### CAD Learnings
This project significantly expanded my feature-based modeling skills:

- I learned how to **add and control text** on complex curved surfaces using embossing and debossing.
- I discovered more efficient ways to create angled surfaces, especially using **chamfer profiles with variable distances**, instead of constructing the geometry manually with arcs or sweeps.
- I gained experience using **parametric patterns**, multi-body modeling, and joint definitions to build assemblies that behave like real products.
- I became more comfortable with **modeling internal components**, which required careful planning to avoid geometry conflicts when assembling them later.

These skills directly translate to more advanced product development and mechanical design work.

---

### Renderings
Below is a rendering of the completed assembly, showcasing the pump, internal tube, and detailed bottle geometry:

**Figure 1. Final Perfume Bottle CAD Model - Front View**  
![Perfume Render](/assets/images/perfume3.jpg)

**Figure 2. Final Perfume Bottle CAD Model - Bottom View**  
![Perfume Render](/assets/images/perfume1.jpg)

---

### Summary
This project demonstrated my ability to reverse-engineer a consumer product and recreate it in CAD with attention to aesthetic details, functional components, and manufacturing realism. It strengthened my understanding of modeling strategy, feature selection, assembly structure, and detailed rendering—skills I continue to apply in subsequent design projects.
