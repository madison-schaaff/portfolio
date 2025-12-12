---
layout: project
title: MAE 4272 Wind Turbine Blade Design Project
description: Advanced CAD + Aerodynamics Project
technologies: [Autodesk Fusion, MATLAB]
image: /assets/images/bladee.jpg
---

### Project Overview
As part of MAE 4272, our team was tasked with designing and experimentally validating a custom wind-turbine blade capable of outperforming the baseline blade geometry tested earlier in the course. The project required producing a blade optimized for **low-Reynolds-number operation**, where aerodynamic performance is highly sensitive to airfoil shape and angle-of-attack control. Our design had to increase power output near a target operating speed of ~1880 RPM while remaining structurally reliable, manufacturable, and fully compatible with the existing hub and wind-tunnel setup. This work combined aerodynamic modeling, structural considerations, CAD design, and hands-on testing (see **Figure 1** for the wind-tunnel configuration).

**Figure 1. Wind Tunnel Test Setup with Custom Blade Installed**  
![Wind Tunnel Photo](https://github.com/madison-schaaff/portfolio/raw/main/assets/images/testing.jpg)


### Design Process
We began by selecting operating parameters of **5 m/s incoming flow**, an optimal **tip-speed ratio of λ ≈ 6**, and a corresponding design speed of **1880 RPM**. Airfoil performance data indicated peak efficiency at approximately **7° angle of attack**, with maximum lift-to-drag ratio near **CL/CD ≈ 66.5**, guiding our selection of twist and chord distribution.

Using **Blade Element Momentum Theory (BEMT)**, we computed inflow angle, relative velocity, and aerodynamic loading at discrete spanwise elements. These calculations were used to size chord, adjust twist, and estimate torque, thrust, and bending stresses. The final geometry balanced aerodynamic efficiency with structural safety—specifically ensuring bending stresses remained below the material limit of roughly **44 MPa**.

**My primary contribution was creating the complete CAD model**, including the custom airfoil profile, full blade geometry, and the hub/attachment interface. This required integrating aerodynamic design outputs with manufacturability constraints and refining the taper and twist distributions into a smooth, printable solid model. The final blade CAD is shown in **Figure 2**, highlighting the aerodynamic planform and root geometry used for attachment.

**Figure 2. CAD Model of Final Blade**  
![CAD Model](https://github.com/madison-schaaff/portfolio/raw/main/assets/images/cad.jpg)

### Testing Summary
The manufactured blade was tested in the MAE wind tunnel across wind speeds of 3–6 m/s using the Lab-4 DAQ system and a torque brake to impose controlled load. During testing, I operated the torque brake, manually adjusting its voltage to sweep through the operating range and recording the corresponding torque and RPM values at each setting. These measurements formed the basis for constructing the blade’s power curve.

As seen in **Figure 3**, the custom blade achieved a high peak power at all wind speeds, consistent with model predictions, which out performed our baseline design. However, the blade exhibited some **startup sensitivity and occasional stall at low Reynolds numbers**, a known challenge when aerodynamic loading is light and the flow is not fully developed. Despite these limitations, structural performance was stable with no observed vibrations, deformation, or mechanical issues during testing.

**Figure 3. Measured Power Curve Compared to Design Point**  
![Power Curve](https://github.com/madison-schaaff/portfolio/raw/main/assets/images/powercurve.jpg)

### My Contribution
Across the project, I was responsible for:
- **Complete CAD development**, including custom airfoil generation, blade geometry, hub design, and preparation of print-ready manufacturing files  
- Integrating BEMT-based aerodynamic targets into a manufacturable 3D model  
- **Operating the torque brake during wind-tunnel tests** and recording experimental torque/RPM data  
- Organizing raw DAQ data for power-curve generation and comparison with BEMT predictions  
- Assisting in diagnosing startup stall behavior and evaluating deviations from theoretical performance  

---


