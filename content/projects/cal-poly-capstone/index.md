---
title: "Home Energy Management System - Cal Poly Capstone Project"
date: 2025-01-01
draft: false
description: "Team Lead & Hardware Engineer for Cal Poly Capstone Project - Comprehensive home energy monitoring system with intelligent EV charging control to prevent electrical panel overloads."
image: "/capstone-expo.jpg"
tags: ["Python", "Embedded Systems", "C++"]
---

### Project Overview
As electric vehicles and household appliances increase energy demand, home electrical panels can become overloaded. This capstone project aims to create a home energy monitoring system that empowers users to track their energy usage and dynamically adjust EV charging rates, helping balance overall power consumption and prevent overloads.

<a href="https://github.com/jhaowen426/OCPP" target="_blank" class="github-button">
    <svg width="16" height="16" viewBox="0 0 16 16" fill="currentColor">
        <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
    </svg>
    View on GitHub
</a>


<img src="/capstone-overview.jpg" alt="Home Energy Management System" style="border: 2px solid #ddd; border-radius: 8px; padding: 10px; box-shadow: 0 2px 4px rgba(0,0,0,0.1); max-width: 100%; height: auto;">
*Capstone Expo Posterboard - Complete system architecture and demonstration*



### Key Responsibilities
- **Team Leadership**: Coordinated efforts across hardware, software, and systems integration
- **Embedded Systems Design**: Designed and implemented a finite state machine (FSM) responsible for translating raw current measurements from a current transformer clamp into actionable charging commands for the EV charger. This system utilized a custom algorithm to dynamically modulate EV charge rates through the Open Charge Point Protocol server using Python.

### Technical Implementation
- **IoT Power Energy Monitor**: Current measurement and serial communication for real-time power monitoring
- **Variac & Step-Down Transformer**: Adjustable AC voltage output and simulated electric panel for testing
- **OCPP Server**: Implemented Open Charge Point Protocol server for standardized EV charging communication
- **Adaptive Control Algorithm**: Developed Python-based state machine for dynamic charging rate adjustment based on current thresholds
- **Hardware Integration**: Successfully integrated multiple hardware platforms (ESP32, Raspberry Pi, Variac, step-down transformer)

<img src="/hardware-diagram.png" alt="Hardware Components" style="border: 2px solid #ddd; border-radius: 8px; padding: 10px; box-shadow: 0 2px 4px rgba(0,0,0,0.1); max-width: 100%; height: auto;">

---

### Experimental Results
The system successfully demonstrated real-time energy monitoring and adaptive control capabilities:

<img src="/experimental-data.png" alt="Experimental Data" style="border: 2px solid #ddd; border-radius: 8px; padding: 10px; box-shadow: 0 2px 4px rgba(0,0,0,0.1); max-width: 100%; height: auto;">

### Outcomes
- Successfully prototyped a working home energy monitoring system on a Tesla Model 3
- Demonstrated real-time power consumption tracking and automatic EV charging rate adjustment
- Delivered comprehensive documentation and system architecture for future development

---
This project represents the culmination of my computer engineering education, combining embedded systems, software development, and real-world industry collaboration to solve critical energy management challenges and make EVs more accessible.





