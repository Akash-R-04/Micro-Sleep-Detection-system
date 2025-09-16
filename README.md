# Micro-Sleep Detection System

A system designed to detect micro-sleeps in real time, by monitoring eye behaviour using sensor / camera + microcontroller, and alerting the user to avoid accidents or mistakes.  

---

## 📌Table of Contents

- 📖 [Overview](#-overview)  
- [✨Features](#-features)  
- [Motivation](#motivation)  
- [Architecture & Components](#architecture--components)  
- [Setup & Installation](#setup--installation)  
- [Usage](#usage)  
- [Screenshots / Figures](#screenshots--figures)  
- [🤝Contributing](#-contributing)  
- [🔮Future Work](#-future-work)  

---

## 📖 Overview

Micro-sleep refers to brief, involuntary episodes of loss of attention which can last a few seconds. The **Micro-Sleep Detection System** aims to monitor signs of fatigue (e.g. prolonged eye closure or nodding) and raise alerts so that users (especially drivers, machine operators etc.) can avoid dangerous lapses in attention.

---

## ✨Features

- Real-time monitoring of eye behaviour  
- Detection of prolonged eye closure or blink patterns indicative of drowsiness  
- Visual/audio alert when micro-sleep is detected  
- Lightweight and deployable on embedded/hardware platforms (e.g. Arduino / microcontroller)  
- Low cost, minimal hardware requirements  

---

## Motivation

- To reduce accidents caused by driver fatigue, especially in long-distance travel, heavy vehicle driving.  
- To support workplace safety where attentiveness is critical (e.g. control rooms, monitoring duty).  
- To explore computer vision / sensor based detection algorithms on resource constrained hardware.

---

## Architecture & Components

| Component | Description |
|-----------|-------------|
| **Sensor / Camera** | Captures eye / face region video/images. |
| **Microcontroller / Processor** | Arduino / compatible board runs code or processes sensor input. |
| **Detection Algorithm** | Code to analyse eye closure, blink rate or other fatigue indicators. |
| **Alert Mechanism** | A buzzer or LED or sound output to notify the user. |

---

## Setup & Installation

> *These instructions assume you have the required hardware components (camera / sensor, microcontroller etc.), and necessary drivers/bindings installed.*

1. Clone the repository:  
   ```bash
   git clone https://github.com/Akash-R-04/Micro-Sleep-Detection-system.git
   cd Micro-Sleep-Detection-system
2. Install dependencies🛠️:
 - If using Arduino, ensure you have the Arduino IDE installed.
 - If using any external libraries (e.g. OpenCV / eye detection models), install them via your package manager (e.g. pip install opencv-python).
3. Upload the firmware / code to your microcontroller. For example, if using the nmit_project.ino, open it in Arduino IDE and upload.
4. Configure any thresholds (e.g. duration of eye-closure, blink rate) in the code to suit your environment / lighting etc.

Usage
1. Power on the system so the camera / sensor starts capturing.
2. Position the camera so it clearly captures the eyes / face of the user.
3. Let the detection algorithm run. It will monitor eye state in real time.
4. When micro-sleep or drowsiness is detected, the system raises an alert (LED / sound / buzzer).

## Screenshots / Figures
Here are some illustrative figures from the repo:


📉 [![Fig1](https://github.com/Akash-R-04/Micro-Sleep-Detection-system/blob/main/fig1.jpg)]()
Dashboard [![Fig2](https://github.com/Akash-R-04/Micro-Sleep-Detection-system/blob/main/fig2.jpg)]()
[![Fig3](https://github.com/Akash-R-04/Micro-Sleep-Detection-system/blob/main/fig3.jpg)]()
📉 [![Fig4](https://github.com/Akash-R-04/Micro-Sleep-Detection-system/blob/main/fig4.jpg)]()

🤝Contributing
Contributions are welcome! 🎉 If you have suggestions, bug fixes, or enhancements:
1. Fork the repository
2. Create a new branch (git checkout -b feature-yourfeature)
3. Make your changes and commit with meaningful messages
4. Push to your branch
5. Open a Pull Request describing what you’ve done

🔮Future Work
Potential improvements or expansions include:
1. More robust facial landmark detection in low light / occlusion
2. Integration with machine learning models for higher-accuracy fatigue detection
3. Adding a mobile app / dashboard for logging & statistics
4. Deploying on smaller, more efficient boards / optimizing for power consumption
