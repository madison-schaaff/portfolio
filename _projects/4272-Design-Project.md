---
layout: project
title: MAE 4272 Wind Turbine Blade Design Project
description: Advanced CAD Project
technologies: [Autodesk Fusion]
image: /assets/images/Stone.jpg
---

### Project Summary
This project focused on designing, analyzing, and experimentally testing a small-scale horizontal-axis wind turbine blade optimized for operation at low Reynolds numbers. Using principles from aerodynamics, blade element momentum theory (BEMT), and structural analysis, our team developed a custom blade geometry intended to outperform the baseline blade used in Lab 4. The final design emphasized aerodynamic efficiency, manufacturability, and structural reliability while remaining within strict experimental and equipment constraints.

### Design Objectives & Constraints
Objectives:
- Maximize aerodynamic efficiency at low Reynolds numbers.
- Improve power output compared to the Lab 4 baseline at the target operating RPM.
- Ensure structural reliability and avoid failure during high-speed operation.
- Maintain a smooth, manufacturable blade geometry compatible with the existing hub.

Constraints:
- Maximum blade length: 6 in
- Minimum axial clearance: < 2 in from the nacelle
- Equipment limits: RPM < 3500, Torque < 3.5 N·cm, wind tunnel speed < 15 Hz (≈9.8 m/s)
- Blade must integrate with the hub attachment piece
- Maximum bending stress must remain < 44 MPa (flexural strength)

### Hypotheses & Assumptions
We expected that a blade with high lift-to-drag ratio, moderate taper, and appropriate geometric twist would maintain near-optimal angle of attack along the span, resulting in peak aerodynamic and power performance near the design RPM.

Assumptions:
- Incoming flow is steady, uniform, and aligned with the rotor axis.
- Torque brake behavior is consistent for gradually increasing loads.
- Mechanical losses are small and effectively constant.
- BEMT provides valid predictions in the low-Re regime.

### Design Process
Our design began by selecting operating parameters of Ur = 5 m/s, λ_opt = 6, and an optimal rotational speed of Ω = 1880 RPM. Airfoil tools data indicated a peak performance at α = 7°, with:
- Max CL/CD = 66.5
- CL = 1.37

Using Blade Element Momentum Theory, we:
- Calculated relative velocity, inflow angle, and angle of attack for each blade element.
- Interpolated airfoil lift and drag coefficients.
- Computed element-level lift, drag, thrust, torque, and contributions to bending stress.
- Integrated along the blade span to estimate total power production and structural safety factor.
- Evaluated performance over a range of wind speeds using a Weibull distribution model.
The resulting blade geometry met all design and structural requirements and was manufactured via 3D printing.

### Experimental Protocol
We planned to collect power curve data for wind speeds from 3–6 m/s using the Lab 4 DAQ system and torque brake. Because the blade was designed for 1880 RPM, we focused on rotational speeds near that target. Safety protocols included strict RPM caps, monitoring for vibrations or unusual sounds, and shutting down the tunnel before adjusting the torque brake.

In practice, the blade experienced challenges initiating rotation, and in some cases stalled before reaching the target RPM. Limited lab time further constrained data collection.

### Results
- The blade showed higher maximum power output than the Lab 4 baseline.
- The structure remained stable with no observed failures.
- Due to startup issues and limited testing time, the collected data exhibited variability.
- A Weibull-weighted performance estimate yielded an expected power of 0.72 W, corresponding to an annual output of 6.3 kWh.

### Reflection
What Went Well:
- Measurable improvement in peak power generation versus the baseline.
- Successful manufacturing and structural performance.

Unexpected Outcomes:
- Actual power was significantly lower than predicted BEMT values.
- Wind tunnel flow often did not settle before data collection, causing inconsistent results.

Challenges:
- Time constraints limited the number of trials and prevented retesting after modifications.
- Startup and stall behavior proved more sensitive than expected at low Reynolds numbers.

### Next Steps
To further refine the design and improve predictive accuracy, the next steps include:
- Collecting a larger dataset across multiple days to eliminate transient turbulence effects.
- Investigating root causes of startup stall (twist distribution, airfoil choice, or hub effects).
- Re-optimizing the blade considering real-world startup behavior rather than ideal BEMT predictions.
- Incorporating dynamic stall models or CFD to improve predictive fidelity.

