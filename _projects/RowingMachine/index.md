---
layout: post
title: The Fly Lever - Air-Damped Resistance Trainer [Capstone 2/Product Design Course Project]
description: A compact, cost-effective athletic assessment tool designed to replicate the dynamic resistance profile of a Concept 2 Dyno using mechanical advantage and fluid drag modeling.
weight: 5
skills: 
  - Mechanism Design
  - SolidWorks (CAD/FEA)
  - Design for Manufacturability (DFM)
  - Cost Analysis (BOM)
main-image: /rowingmachine.jpg
---

## Project Overview
Commissioned to support NextGen athletic coaches, this project aimed to bridge the gap between high-end performance data and equipment portability. The industry standard, the Concept 2 Dyno, is often prohibitively expensive ($5,000+) and bulky. 

Our team developed "The Fly Lever"—a resistance machine that utilizes an air-damped flywheel to provide a smooth, gradual increase in force that replicates the feeling of rowing. The project was completed under a strict budget while maintaining professional-grade durability and data reproducibility.

---

## Technical Architecture & Design

### 1. Drivetrain & Mechanical Advantage
The primary mechanical challenge was converting the slow, high-torque pull of a human user into the high-velocity rotation required for air-damping.
* **Gear Ratio:** We implemented a 4:1 ratio using a 15-tooth to 60-tooth sprocket system. This allows the flywheel to reach the high RPMs necessary to generate significant drag.
* **The Freewheel Mechanism:** To ensure user safety, a freewheel sprocket was integrated into the drive hub. This allows the flywheel’s momentum to dissipate safely without "snapping" the lever arms back toward the user at the end of a stroke.


### 2. Fluid Drag & Resistance Modeling
Unlike weight-based resistance, the Fly Lever uses air resistance, which scales quadratically with velocity.
* **Fan Blade Geometry:** We designed custom CNC-machined ABS fan blades with a specific C-shaped geometry to capture air efficiently.
* **Physics Validation:** Through mathematical modeling, we generated Torque vs. Velocity curves to ensure the resistance profile matched the "feel" required for explosive power training.


### 3. Design for Manufacturability (DFM)
* **Material Selection:** The frame was constructed from 6061 Aluminum to maximize the strength-to-weight ratio, ensuring the device remains portable.
* **Ergonomics:** A pin-locking seat mechanism was designed to accommodate a wide range of athletes, from 5'0" to 7'0" in height.
* **Technical Documentation & GD&T:** Produced production-ready SolidWorks drawings applying GD&T principles to define critical tolerances for the high-RPM flywheel and CNC-machined components, ensuring precise fitment and assembly reliability.
{% include image-gallery.html images="rowingdrawing1.jpg" height="400" %}

---

## Documentation & Results
* **Dynamic Resistance Analysis:** Documented the mathematical relationship between user input force and flywheel RPM.
* **Manufacturing Package:** Produced a full Bill of Materials (BOM) and 2D engineering drawings with proper GD&T for all custom components.
* **Cost Efficiency:** Successfully delivered a functional design at ~50% of the cost of current market competitors.
