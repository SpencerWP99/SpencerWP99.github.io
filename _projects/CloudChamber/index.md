---
layout: post
title: Portable Handheld Cloud Chamber
description: A compact, battery-powered particle detector designed for educational demonstrations, utilizing thermoelectric cooling and custom PCB control to visualize ionizing radiation in real-time.
weight: 4
skills: 
  - Prototyping & Assembly
  - Thermoelectric Cooling (TEC)
  - PCB Design (Altium/KiCad)
  - Power Electronics
main-image: /cloudchamber.jpg
---

## Project Overview
Commissioned by a University Professor, this Capstone project aimed to miniaturize a traditionally bulky laboratory instrument into a handheld device. The Cloud Chamber allows students to observe alpha and beta particles by creating a supersaturated environment of Isopropyl Alcohol (IPA) vapor, where radiation tracks become visible to the naked eye.

The primary engineering challenge was achieving the extreme temperature gradient required for cloud formation within a portable, battery-efficient footprint.

{% include youtube-video.html id="23r60XFx7H8" autoplay="false" width="100%" %}

---

## Technical Architecture & Design

### 1. Thermal Management & The Peltier Effect
The heart of the device is a **Peltier Device (Thermoelectric Cooler)**.
* **Cold Side:** Achieved sub-zero temperatures to create the "sensitive volume" where alcohol vapor condenses around radiation tracks.
* **Hot Side:** Utilized an active cooling system consisting of a high-efficiency heat sink and a variable-speed fan to dissipate waste heat, preventing thermal runaway and maintaining the necessary temperature gradient.

### 2. Saturated Vapor Environment
* **IPA Saturation:** Sponges are used to hold Isopropyl Alcohol, which is then naturally evaporated by the environment temperature at the top of the chamber to extend the saturation state.
* **Condensation Zone:** As the vapor falls toward the Peltier-cooled base, it becomes supersaturated—the critical state required for particle visualization.

## 3. Custom PCB & Control Systems
* **Closed-Loop Cooling:** Integrated fan speed control to balance thermal dissipation with battery life, ensuring the device remains handheld-safe during extended demonstrations.
* **User Interface:** Developed a simplified control scheme for the professor to toggle power and adjust visibility settings on the fly.

* **Thermal Performance Analysis:** Documented the time-to-cool metrics and steady-state temperature data.
* **Electrical Schematics:** Full documentation of the PCB layout, component selection for the power stages, and wiring diagrams.
* **Operational Guide:** A user manual designed for non-engineering faculty to operate and maintain the chamber, including IPA refueling and safety protocols.

> **Impact:** The final prototype successfully demonstrated visible radiation tracks within 2 minutes of activation, providing the professor with a portable, durable tool for classroom engagement.
