# Transmission_line_faultDetection_system
Transmission Line Fault Detection with Fire Alarm and Protection System
Overview

This project presents a DC transmission line protection system that detects electrical faults and fire hazards in real time. The system continuously monitors transmission line conditions using sensors and automatically isolates faulty sections to prevent damage or accidents.

The system is built using an Arduino microcontroller, current sensor, flame sensor, relay module, and LCD display. It detects abnormal conditions such as line-to-line faults, line-to-ground faults, and overheating/fire hazards, alerts the user, and disconnects the affected line.

A key feature of the project is the fault distance estimation, which helps identify where along the transmission line the fault occurred, allowing faster maintenance and improved safety.

Features

Real-time monitoring of transmission line conditions

Detection of line-to-line faults

Detection of line-to-ground faults

Fire and overheating detection

Automatic relay-based protection

Fault distance estimation

Visual and audible alerts

LCD display for system status

Hardware Components

Arduino UNO / Arduino Nano

ACS712 Current Sensor

Flame Sensor

Relay Module

16×2 LCD Display with I²C Module

Buzzer

LED Indicators

Resistors

Transmission line model (copper wires and towers)

Technologies Used

Arduino IDE

Embedded C / Arduino Programming

Sensor interfacing

Electrical fault detection logic

Microcontroller-based automation

System Working

The system continuously reads current, temperature, and flame sensor values.

The Arduino compares these readings with predefined threshold values.

If abnormal conditions are detected:

The system identifies the type of fault.

The fault distance is estimated.

The relay trips to disconnect the faulty section.

The LCD displays fault information.

LED and buzzer alerts notify the user.

Fault Conditions Detected
Line-to-Line Fault

Occurs when abnormal current flows between two conductors.

Line-to-Ground Fault

Occurs when a conductor directly connects to ground.

Overheating / Fire Fault

Detected using temperature and flame sensors when the temperature crosses a safe limit or flame is detected.

Transmission Line Model

The prototype uses a scaled-down transmission line model:

Four copper wires act as conductors.

Three wires represent phase conductors (R, Y, B).

One wire represents neutral/ground return.

Miniature transmission towers built from ice-cream sticks simulate real transmission towers.

This setup allows:

Fault injection at different points

Demonstration of current behavior during faults

Practical understanding of power system protection

Block Diagram Workflow

Start system

Initialize sensors and LCD

Read current and temperature values

Compare readings with thresholds

If normal → continue monitoring

If fault detected →

Identify fault type

Estimate fault distance

Trip relay

Display alert on LCD

Activate buzzer and LED

Applications

Power system protection studies

Educational demonstration of transmission line faults

Smart monitoring systems

Electrical safety systems

Future Improvements

IoT-based remote monitoring

GSM alerts for fault notification

Mobile app interface

More accurate fault distance calculation

Integration with smart grid systems

Team Members

Saurabh Mishra

Pratiksha Kaushal

Isha Bhadauria

Krishna

Manish Pradhan

Mohit Meena
