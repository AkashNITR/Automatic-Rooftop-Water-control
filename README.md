# Automatic Rooftop Water Tank Control System

## Overview
An automated system leveraging an 8051 microcontroller to monitor and control rooftop water tank levels. It ensures water management efficiency and reduces manual intervention by automatically managing the motor pump based on water levels.

## Features
- Automated pump control based on water levels.
- Real-time feedback on system status via LCD display.
- Prevents water wastage and ensures adequate availability.
- Easy integration and scalability for IoT-based remote monitoring.

## Hardware Requirements
- **Microcontroller:** AT89C52 (8051 family)
- **Sensors:** Float sensors for water level detection
- **Actuators:** 5V DC submersible pump controlled via L293D motor driver
- **Power Supply:** 9V DC external source
- **Others:** LCD display, op-amp IC741, resistors, jumper wires

## Detailed component list
![{347E1822-82A4-48FE-838A-098D85D5B6BA}](https://github.com/user-attachments/assets/7cefdefa-a54b-42e7-8d04-a43ac5735819)

## Firmware
The firmware includes logic to:
1. Read water levels from sensors.
2. Control the pump based on defined operational states.
3. Display real-time system status.

## Circuit Diagram
![Screenshot 2024-11-27 214731](https://github.com/user-attachments/assets/5bf0ad3c-7e45-4eff-81dc-69a6a76c1f27)

**Programed in Proteus**

## How to Use
1. Assemble the circuit as per the diagram.
2. Flash the firmware onto the AT89C52 microcontroller using a compatible programmer.
3. Power the system with the external DC source.
4. Monitor and test the system under different water levels.

## Test Results
| **Top Sensor** | **Bottom Sensor** | **Previous State** | **Current State** |
|----------------|-------------------|---------------------|-------------------|
| 0              | 0                 | X                   | 1                 |
| 0              | 1                 | 0                   | 0                 |
| 0              | 1                 | 1                   | 1                 |
| 1              | 1                 | X                   | 0                 |
