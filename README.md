# Remote-Controlled Tesla – 

This repository contains the source code and hardware schematics for the **Remote-Controlled Tesla** project developed by **The Golden Dragon Team**. As the lead programmer, I was responsible for implementing the core logic, including motor control, Bluetooth communication, and LED management.

---

## Overview

The objective of this project was to design and build a Bluetooth-controlled car that can move in all directions and toggle LED lights remotely. The car is controlled via an Android application using Bluetooth communication, allowing for real-time interaction and control.

**Key Features:**
- Bluetooth control using HC-05 module
- Four-wheel drive using L298N motor driver
- Directional commands: forward, backward, left, right, stop
- Remote-controlled LED toggling
- Modular object-oriented Arduino code

---

## Technical Specifications

**Hardware**
- Microcontroller: Arduino Uno
- Motor Driver: L298N Dual H-Bridge
- Bluetooth Module: HC-05
- Motors: 4 x DC gear motors
- Power Supply: 7.4V Li-ion battery with voltage regulator
- LED: Connected to digital pin 13 (external or onboard)

**Connections**
- HC-05 RX → Arduino TX  
- HC-05 TX → Arduino RX  
- HC-05 VCC → Arduino 5V  
- HC-05 GND → Arduino GND  
- ENA → D9  
- IN1 → D8  
- IN2 → D7  
- IN3 → D6  
- IN4 → D5  
- ENB → D3  
- LED anode → D13  
- LED cathode → GND

**Software**
- Language: Arduino C++
- IDE: Arduino IDE
- Control App: Arduino Bluetooth Controller (Android)
- Commands:
  - `F` – Forward
  - `B` – Backward
  - `L` – Turn Left
  - `R` – Turn Right
  - `S` – Stop
  - `1` – LED ON
  - `0` – LED OFF

---

## Repository Structure

```
Remote-Controlled-Tesla/
├── Arduino Control/          # Arduino sketches and logic modules
├── Designs/                  # CAD designs and schematics
├── README.md                 # Project overview
```

---

## Achievements

- Successfully implemented Bluetooth communication for remote control
- Calibrated all four motors for synchronized movement
- Integrated LED control via Bluetooth commands
- Developed modular and maintainable codebase
