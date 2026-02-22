---
layout: post
title: 2. High-Speed Mechatronic Sorting System [University Project]
description: A real-time control and classification system developed to automate the high-speed sorting of multi-material cylinders using an ATmega2560 and custom C-based firmware.
skills: 
  - Embedded Systems (C/C++)
  - Embedded Systems
  - Control Algorithms
main-image: /sortmachine.jpg
---

## Project Overview
For this capstone-level mechatronics project, I developed the control architecture and embedded software to manage a school-provided mechanical sorting assembly. The goal was to sort 48 material-diverse cylinders (Black Plastic, White Plastic, Steel, and Aluminum) with maximum throughput. 

Operating on a dual-motor hardware platform—featuring a DC-driven conveyor and a stepper-actuated tray—my implementation achieved a throughput of **30 seconds with 100% accuracy**, significantly exceeding the project's performance benchmarks of <60 seconds with 95% accuracy.

{% include youtube-video.html id="okAGCAGFZ-Y" autoplay="false" width="100%" %}

---

## Embedded Architecture & Electrical Interfacing
I designed the electrical interface and signal-processing logic to bridge the gap between the school's mechanical components and an ATmega2560 microcontroller.

* **Sensing Suite Integration:** I developed the ADC sampling and classification algorithms for the system's infrared reflectivity sensors and optical gates. This involved implementing software filters to mitigate sensor noise caused by DC motor vibration.
* **Firmware-Based Motion Control:** I programmed the motion control logic for the stepper motor, utilizing an **s-curve acceleration profile** to manage inertial loads during high-speed indexing.

---

## Software Optimization & Logic
To maximize the system's sorting efficiency, I engineered several novel firmware-level enhancements:

### 1. Adaptive Throughput (Variable PWM)
I optimized the loading phase by implementing a dual-speed belt logic. The firmware drives the conveyor at **50% duty cycle** when the item queue is empty to accelerate loading, and automatically drops to **25%** once items reach the classification zone to ensure high ADC sample counts for accurate material identification.

### 2. High-Precision Timing Firmware
I modified the system’s low-level timing functions to increase resolution from 1ms to **10µs**. This precise control enabled the fine-tuning of stepper motor acceleration and deceleration ramps, which was critical to achieving the 30-second completion time.

### 3. FIFO Buffer & State Machine
Items are tracked through a **First-In-First-Out (FIFO) linked-list queue**. I developed a robust state machine in C that handles interrupt-driven transitions between classification, tray rotation, and belt indexing.
