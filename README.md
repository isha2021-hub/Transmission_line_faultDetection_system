# Transmission_line_faultDetection_system
# Transmission Line Fault Detection with Fire Alarm and Protection System

## Overview
This project presents a DC transmission line protection system that detects electrical faults and fire hazards in real time. The system continuously monitors transmission line conditions using sensors and automatically isolates faulty sections to prevent damage or accidents.

The system is built using an Arduino microcontroller, current sensor, flame sensor, relay module, and LCD display. It detects abnormal conditions such as line-to-line faults, line-to-ground faults, and overheating or fire hazards, alerts the user, and disconnects the affected line.

A key feature of the project is fault distance estimation, which helps identify where along the transmission line the fault occurred, allowing faster maintenance and improved safety.

---

## Features
- Real-time monitoring of transmission line conditions
- Detection of line-to-line faults
- Detection of line-to-ground faults
- Fire and overheating detection
- Automatic relay-based protection
- Fault distance estimation
- Visual and audible alerts
- LCD display for system status

---

## Hardware Components
- Arduino UNO / Arduino Nano
- ACS712 Current Sensor
- Flame Sensor
- Relay Module
- 16×2 LCD Display with I2C Module
- Buzzer
- LED Indicators
- Resistors
- Transmission line model (copper wires and towers)

---

## Technologies Used
- Arduino IDE
- Embedded C / Arduino Programming
- Sensor interfacing
- Microcontroller-based automation
- Electrical fault detection logic

---

## System Working
1. The system continuously reads current and flame sensor values.
2. The Arduino compares these readings with predefined threshold values.
3. If abnormal conditions are detected:
   - The type of fault is identified.
   - The fault distance is estimated.
4. The relay trips to disconnect the faulty section.
5. The LCD displays the fault information.
6. LED indicators and buzzer notify the user.

---

## Fault Conditions Detected

### Line-to-Line Fault
Occurs when abnormal current flows between two conductors.

### Line-to-Ground Fault
Occurs when a conductor directly connects to ground.

### Fire / Overheating Fault
Detected using a flame sensor when fire or abnormal heat is detected near the transmission line.

---

## Transmission Line Model
The prototype uses a scaled-down transmission line model:

- Four copper wires act as conductors.
- Three wires represent the R, Y, and B phases.
- One wire represents neutral or ground.
- Miniature towers built using ice-cream sticks simulate real transmission towers.

This setup allows fault injection at different points and demonstrates current behavior during faults.

---

## Project Workflow
Start System
↓
Initialize Sensors and LCD
↓
Read Current and Flame Sensor Values
↓
Compare Readings with Threshold
↓
If Normal → Continue Monitoring
↓
If Fault Detected
↓
Identify Fault Type
↓
Estimate Fault Distance
↓
Trip Relay and Display Alert

---

## Applications
- Power system protection studies
- Educational demonstration of transmission line faults
- Smart monitoring systems
- Electrical safety systems

---

## Future Improvements
- IoT-based remote monitoring
- GSM alerts for fault notification
- Mobile application interface
- Improved fault distance calculation
- Integration with smart grid systems

---

## Team Members
- Saurabh Mishra  
- Pratiksha Kaushal  
- Isha Bhadauria  
- Krishna  
- Manish Pradhan  
- Mohit Meena
