---
layout: project
title: MAE 2250 Cord Roller Project
description: Product Design, CAD, and Prototyping
technologies: [Autodesk Fusion, FDM 3D Printing]
image: /assets/images/roller.jpg
---

### Project Overview
For my MAE 2250 final project, I designed and engineered a compact cord-management device—later named the **Cord Cubby**—intended to solve the everyday problem of tangled chargers, earbuds, and USB cables. My goal was to create a small, reliable, user-friendly mechanism that could neatly spool a cord into an enclosed housing while remaining durable enough for daily use and portable enough to fit comfortably in a backpack or pocket.

This project involved the full engineering design cycle: concept generation, rapid prototyping, CAD modeling, mechanical testing, redesign, and fabrication of a functional final product.

---

### Ideation & Early Prototyping
I began by brainstorming a wide range of mechanisms—spring-loaded reels, hinged spools, collapsible housings, and friction-based winders. From these, I selected three concepts to prototype based on feasibility, manufacturability, and functional potential.

Below are the three rough prototypes I built using inexpensive materials such as cardboard, tubes, clips, rope, and tape:

**Figure 1. Prototype A — Vertical Tube Spool Concept**  
![Prototype 1](/assets/images/p1.jpg)

**Figure 2. Prototype B — Sliding Box & Coil Mechanism (Selected for Development)**  
![Prototype 2](/assets/images/p2.jpg)

**Figure 3. Prototype C — Dual-Disk Clamp Spool**  
![Prototype 3](/assets/images/p3.jpg)

To choose which prototype to move forward with, I performed three categories of tests on each:

- **Functionality tests:** How smoothly the mechanism wound and released a cord  
- **Durability tests:** Structural robustness under repeated loading and drop tests  
- **Reliability tests:** Consistency of operation after multiple cycles  

**Prototype B**—the sliding box and internal spool design—outperformed the others in all three categories. It offered the best balance of compactness, controllability, manufacturability, and user familiarity, so I selected it as the foundation for the final device.

---

### CAD Development & Mechanism Design
After selecting the mechanism, I transitioned into full CAD development in Autodesk Fusion. I modeled all internal and external components, including:

- A **central rotating shaft** with a clip to secure the cord end  
- A **spool geometry** optimized for even winding  
- A two-part **outer enclosure** with smooth edges for pocket-safe handling  
- A **magnet-and-post alignment system** to secure the lid without fasteners  
- A **finger-operated dial** that allows the user to wind the cord easily

From my final report, I incorporated several manufacturing and assembly considerations into the CAD:

- Added **0.5 mm tolerances** based on ABS 3D printing constraints :contentReference[oaicite:0]{index=0}  
- Eliminated overly tight features that previously required drilling or sanding  
- Replaced the fragile fold-out crank with a simpler, more reliable finger slot  
- Reduced the number of magnets from six to two and supplemented them with alignment posts  
- Ensured all features could be fabricated without complex molds, consistent with design-for-manufacturing principles

---

### Full-Scale Fabrication & Testing
I fabricated the first full-scale Cord Cubby using FDM 3D printing in ABS plastic. The initial print revealed several important insights:

- **Magnet holes printed undersized**, requiring redesign for improved tolerances  
- The **shaft–lid interface needed additional clearance** to avoid friction binding  
- Printed clips were fragile, prompting a shift to off-the-shelf components

I then performed a second round of structured tests:

#### **1. Functionality Testing**
- Evaluated smoothness of winding  
- Confirmed cord compatibility across multiple cable types  
- Verified ergonomic performance of the finger-rotation slot  

#### **2. Durability Testing**
- Conducted drop tests and repeated winding cycles  
- Identified stress concentrations near magnet pockets (later reinforced)  

#### **3. Reliability Testing**
- Measured consistency over 25+ winding cycles  
- Ensured the lid maintained alignment during operation  

Informed by these results, I iterated the design once more—reinforcing the lid attachment points, tightening the housing size, and smoothing internal surfaces to reduce friction.

---

### Final Product
Below is the final 3D-printed Cord Cubby and its CAD model after all refinements:

**Figure 4. Final Cord Cubby — ABS Fully Assembled Unit**  
![Final Product](/assets/images/final.jpg)

**Figure 5. Final Cord Cubby — CAD Model**  
![Final Product CAD](/assets/images/roller.jpg)

The final design is compact, lightweight, and simple to operate. The magnetic/post hybrid closure system holds the lid securely, the central clip reliably anchors the cord, and the rotating shaft allows the device to wrap cords quickly and neatly. ABS plastic provides a strong balance of durability and low weight, making the product suitable for everyday transport.

---

### Reflection
This project taught me how to translate an early conceptual idea into a refined, manufacturable product. I learned how to:

- Use CAD not just to model geometry, but to solve assembly and manufacturing constraints  
- Apply design-for-manufacturability and design-for-assembly principles  
- Rapidly prototype and test mechanisms to make evidence-based design decisions  
- Incorporate tolerancing and fit considerations into 3D printed parts  
- Iterate through multiple cycles of testing and refinement to achieve reliability  

Overall, the Cord Cubby project gave me hands-on experience with mechanical design, user-focused engineering, rapid prototyping, and structured product testing—skills that directly translate to real-world engineering environments.

