<!-- ===================== HEADER ===================== -->

<div align="center">

# Speed-Adaptive Long-Range Proximity Warning System

### Driver Assistance System for Real-Time Safe Following Distance Detection

![Status](https://img.shields.io/badge/Status-In%20Development-yellow)
![Platform](https://img.shields.io/badge/Platform-Embedded%20System-blue)
![Language](https://img.shields.io/badge/Language-C%20%7C%20C%2B%2B%20%7C%20Python-orange)
![Hardware](https://img.shields.io/badge/Hardware-Custom%20Prototype-red)
![Budget](https://img.shields.io/badge/Budget-%24240%20per%20student-green)

</div>

---

<!-- ===================== BANNER ===================== -->

<p align="center">
  <img src="docs/images/project-banner.png" 
       alt="Speed-Adaptive Long-Range Proximity Warning System Banner"
       width="100%">
</p>

---

## Executive Summary

Rear-end collisions can occur when drivers fail to recognize that a vehicle ahead is decelerating, particularly during extended highway driving where fatigue, distraction, or delayed reaction can increase stopping risk. Traditional proximity warning systems may rely on fixed distance thresholds that do not adequately account for changing vehicle speeds and relative motion.

This project develops a **Speed-Adaptive Long-Range Proximity Warning System for Driver Assistance**. The system continuously monitors the host vehicle's speed, the relative motion of a leading vehicle, and the distance between the vehicles to determine whether the current following distance is safe.

Unlike a fixed-distance warning system, the proposed approach dynamically determines the required safe following distance based on vehicle speed and relative motion. This allows the warning threshold to adapt to changing driving conditions.

---

## System Overview

The proposed system consists of four primary functions:

```text
┌────────────────────┐
│  Long-Range Sensor │
│                    │
│ LiDAR / IR /       │
│ Ultrasonic /       │
│ Computer Vision    │
└─────────┬──────────┘
          │
          ▼
┌────────────────────┐
│ Sensor Interface   │
│ & Signal           │
│ Conditioning       │
└─────────┬──────────┘
          │
          ▼
┌────────────────────┐
│ Embedded Controller│
│                    │
│ Data Acquisition   │
│ Speed Processing   │
│ Distance Processing│
└─────────┬──────────┘
          │
          ▼
┌────────────────────┐
│ Safe-Distance      │
│ Algorithm          │
│                    │
│ Speed + Relative   │
│ Motion + Distance  │
└─────────┬──────────┘
          │
          ▼
┌────────────────────┐
│ Warning System     │
│                    │
│ Audible Alert      │
└────────────────────┘
