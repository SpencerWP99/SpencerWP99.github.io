---
layout: post
title: Remy - Automated Salad Assembly Robot
description: A complex electro-mechanical system designed to automate salad production and solve the challenges of the current day restaurant industry
skills: 
  - Mechatronics System Design
  - Product Design Cycle
  - Rapid Prototyping
  - Lifecycle Testing
  - Data Analysis
  - Control Algorithms
  - DFMA
  - Leadership/Responsability
main-image: /remy.jpg
---

## Remy Project Overview
Remy is an automated salad-and-bowl production robot designed to solve the challenges of speed, consistency, and sanitation in commercial kitchens. As a core member of the engineering team at [Cibotica](https://cibotica.com), I led/contributed to the mechanical design and development of Remy, primarily the four core modules that drive the system: the vibration-based ingredient dispensers, a magnetic conveyor, a bowl denester, and a synchronized bowl elevator. My work involved taking these subsystems from initial first-principles sketches through to pilot-ready hardware.

{% include youtube-video.html id="EaUrFaaEMco" autoplay="false" width="100%" %}

---

## Remy Lifecycle: From P.O.C to Pilot
My involvement spanned the full product development lifecycle, moving from experimental R&D prototyping to a polished, pilot-ready product.

* **Proof of Concept (P.O.C.):** Very early stage concept version of the robot, a "skeleton" model made from 80-20 extrusion for the frame used to quickly prototype various revisions of each core module + test the concept of a salad-assembly robot, I help with finalizing the concepts through vigorous testing and initial data-logging
* **Alpha Phase/Pre-Pilot:** The first "real" robot; Alpha was designed as the pre-pilot model used for validating core functionality and gauging the restaurant industry's interest in the product. During this stage, I contributed to: finalizing the design of the ingredient dispenser containers and vibration module, and the bowl denester; assembling and mounting the structural framework to the main refrigeration unit; and developing the core modules through rapid prototyping and testing
* **Beta Phase/Pilot Unit:** The pilot unit set to launch in the Vancouver based restaurant Food Republic; the unit would be a case study to prove the sales metrics of the unit and gain outreach for Cibotica. As one of the lead engineers, I lead the redesign from the pre-pilot to production for the ingredient dispenser, the bowl denester, and the bowl elevator + worked with the CTO to redesign the magnetic conveyor and the high-level architecture of Remy. On top of the design cycle, I also contributed to the assembly of the structural architecture and all modules, tested all systems for lifecycle and failure cases + rigorous ingredient testing to prove the modules's agnostic ingredient dispensing and the optimized speed/accuracy metrics of each ingredient, and wrote all the documentation for the Beta unit. More information on the Beta unit specifics can be read below.

{% include image-gallery.html images="teampic.jpg" height="400" %}

---

## Ingredient Dispenser (Patented)
### Lead Designer
A modular assembly designed to dispense any type of ingredient into a bowl at 3-5% accuracy within 15-30 seconds; uses eccentric rotation to create linear motion to vibrate the container at various frequencies based on the speed of output from the weight gate device. I designed the vibration module, the weight gate device, the ingredient containers, and the secondary systems (container weighting system, bowl detection system); the device was designed to be modular and following DFMA principles so third-party technicians could easily swap dispensers on-site without blocking restaurants during operation + each systems was designed to meet NSF/ANSI 2023 food safety standards.

Patent: [WO2024243703 - SYSTEMS, METHODS, AND DEVICES FOR FOOD DISPENSING](https://patentscope.wipo.int/search/en/detail.jsf?docId=WO2024243703&_cid=P21-M66ZFZ-51674-1)

{% include image-gallery.html images="dispenser.jpg" height="400" %}

--

## Bowl Denester
### Lead Designer
The bowl denester dispenses salad bowls onto the magnetic conveyor trays with high precision and accuracy with several backup systems to notify operators of minor issues to prevent system failure. I engineered a linearly-actuated bowl denester that utilizes "ratchet-and-pawl" style fingers to separate nested bowls; the denester is the first action of the system, and failure to denest a bowl would cause every other system to fail, so several secondary modules are designed to prevent edgecases and human error. A bowl catch-lock device was added to prevent bowls from bypassing the force-actuated gate holding the bowl stack and sensors to detect the remaining number of bowls in the stack + to measure the bowl position relative to the conveyor trays to determine if the bowl became misaligned during the final freefaall.

{% include image-gallery.html images="bowldispenser.jpg" height="400" %}

---

## Bowl Elevator
### Lead Designer
A dual-column chain-driven elevator with mirrored kinematics to lift salads from the conveyor tray to the top of the device for operators to finish the garnish and serve; two independent columns with set of arms to grab the bowls, synchronized via proximity sensors and homing algorithms. I designed the drivetrain and chain w/ bowl arms and the sensors for synchronization, bowl detection, and error detection.

{% include image-gallery.html images="bowlelevator.jpg" height="400" %}

---

## Magnetic Conveyor System
To meet strict food safety standards and reduce the cleaning time of the robot, a magnetic conveyor was designed to move bowl trays from module to module seamlessly while allowing the bowls to be quickly removed and washed; the system is design to move bowls incrementaly in a square pattern using electromagnets on hidden rails. I contributed to designing the proof of concept for the rail system and bowl trays, and aided with resolves several issues during testing, such as finding a method to increase the electromagnetic force during the forward motion without incedentally increasing the permanent magnet force during the backwards motion.

{% include image-gallery.html images="conveyor.jpg" height="400" %}

---

## Engineering Knowledge Base & Documentation
To support the transition from R&D to pilot production, I architected and authored the comprehensive documentation database. This was a critical business-focused initiative to ensure that as the company scaled, engineering knowledge was preserved and assembly could be offloaded to manufacturing technicians.

**Key resources:**

* **ALTT (Accelerated Lifecycle Testing):** Authored detailed testing plans, excel data-logging tools and findings to provide data-driven reliability projections for every mechanical module.
* **Assembly Guides & QC Testing:** Created step-by-step visual assembly manuals and Quality Control checklists to ensure consistency across multiple robot builds.
* **Troubleshooting Guides:** Developed logic-based troubleshooting trees to minimize downtime during testing and operation for operators/technicians.
* **Ingredient Testing:** Developed Excel files to analyze data measurements from ingredient testing to output suggestions for optimizing the ingredient dispenser's PD controller.

{% include image-gallery.html images="documentation.jpg" height="400" %}
