---
layout: post
title: Remy - Automated Salad Assembly Robot
description: A complex electro-mechanical system designed to automate fresh food production. Remy utilizes four primary mechatronic modules to handle bowls and dispense ingredients with high precision and sanitation.
skills: 
  - Mechatronics System Design
  - Mechanism Architecture
  - Rapid Prototyping
  - Electromagnetics
  - Control Algorithms
  - DFMA
  - FEA/CFD Simulation
main-image: /remy.jpg
---

## Remy Project Overview
Remy is an automated salad-and-bowl production robot designed to solve the challenges of speed, consistency, and sanitation in commercial kitchens. As a core member of the engineering team at [Cibotica](https://cibotica.com), I led the mechanical design and development of the four primary modules that drive the system: a magnetic conveyor, a bowl denester, a vibration-based ingredient dispenser, and a synchronized bowl elevator. My work involved taking these subsystems from initial first-principles sketches through to pilot-ready hardware.

{% include youtube-video.html id="EaUrFaaEMco" autoplay="false" width="100%" %}

---

## Remy Lifecycle: From Alpha to Beta
My involvement spanned the full product development lifecycle, moving from high-risk experimental R&D to a polished, pilot-ready product.

* **Alpha Phase (Concept & Proof of Concept):** I focused on rapid iteration and risk mitigation. During this stage, I utilized 3D printing and off-the-shelf components to validate the core "physics" of the robot—specifically testing the feasibility of moving magnetic trays through solid stainless steel.
* **Beta Phase (Refinement & Pilot Production):** I transitioned the designs into manufacturable units. This involved rigorous **DFMA** (Design for Manufacturing and Assembly) to reduce part counts, sourcing CNC and sheet-metal components from external vendors, and implementing high-level feedback loops in the firmware.

{% include image-gallery.html images="teampic.jpg" height="400" %}

---

## Ingredient Dispenser (Patented) - Lead Designer
I developed a vibration-based dispensing module capable of handling a wide variety of food textures. The system uses a Horizontal Vibration Module (HVM) to convert rotational motor motion into a pendulum-style oscillation via an eccentric cam and linear rails.

**Key Innovation:** To achieve high-accuracy portioning, I designed a "floating" weight gate isolated from the vibration source. This allows integrated loadcells to measure ingredient mass in real-time without interference from the horizontal oscillation.

Patent: [WO2024243703 - SYSTEMS, METHODS, AND DEVICES FOR FOOD DISPENSING](https://patentscope.wipo.int/search/en/detail.jsf?docId=WO2024243703&_cid=P21-M66ZFZ-51674-1)

{% include image-gallery.html images="dispenser.jpg" height="400" %}

--

## Bowl Denester - Lead Designer
I engineered a linearly-actuated bowl dispenser that utilizes a "ratchet-and-pawl" logic to separate nested bowls. The system features unidirectional spring fingers and a force-actuated gate with adjustable spring tension. 

**Key Innovation:** To maintain consistent performance regardless of stack height, I designed eccentric cams that isolate the weight of the upper bowl stack, ensuring the dispensing mechanism only interacts with a constant load of ~6 bowls.

{% include image-gallery.html images="bowldispenser.jpg" height="400" %}

---

## Bowl Elevator - Lead Designer
To deliver finished bowls to the operator, I designed a dual-column chain-driven elevator. This system features mirrored kinematics where two independent columns are synchronized via proximity sensors and homing algorithms. 

**Key Innovation:** I implemented a 1:4 ratio gear train on NEMA stepper motors to provide the necessary torque for lifting high-capacity bowls while maintaining a slim mechanical footprint.

{% include image-gallery.html images="bowlelevator.jpg" height="400" %}

---

## Magnetic Conveyor System
To meet strict food safety standards, I designed a seamless, wipeable stainless steel floor that houses a hidden magnetic conveying system. I developed a unique "Pull-Repel" cycle using electromagnets and H-bridge PCB revisions to index 3D-printed trays across the surface without any mechanical penetrations. 

**Key Innovation:** To ensure serviceability, I integrated a lift-assist frame supported by calibrated gas springs, allowing the entire internal assembly to be lifted 1.5ft for easy maintenance access.

{% include image-gallery.html images="conveyor.jpg" height="400" %}

---

## System Integration & Testing
Beyond hardware design, I developed the assembly and testing procedures for every subsystem. I created structured data-logging tools in Excel to track lifecycle testing and performance metrics, allowing the team to identify and mitigate design risks before deploying the robot to pilot locations.
