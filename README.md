# SmartDustbinUsingQAM
Designed an ESP32-based smart waste bin with automated lid control using IR sensing, fill-level monitoring via an ultrasonic sensor, and toxic gas detection using an MQ-2 sensor. Provides real-time LCD feedback and wireless alerts, with MATLAB-based analysis of usage patterns.

# Smart Waste Bin Monitoring System (ESP32)

## Overview
ESP32-based smart waste bin system that automates lid control, monitors bin fill level and toxic gases, and sends real-time alerts. The project focuses on embedded system design, sensor interfacing, and reliable real-time operation, with offline MATLAB-based analysis of sensor data.

## Why this project matters
- Demonstrates real-time embedded control
- Practical sensor interfacing and actuation
- End-to-end hardware and firmware integration
- ESP32-based wireless communication
- Basic signal analysis of sensor data

## Hardware Used
- ESP32-WROOM-32E
- HC-SR04 Ultrasonic Sensor
- IR Proximity Sensor
- MQ-2 Gas Sensor
- Servo Motor
- 16×2 LCD Display

## System Architecture
![Block Diagram](hardware/block_diagram.png)

## Firmware Design
- State-based control logic
- Periodic sensor sampling
- Threshold-based decision making
- Peripheral interfacing using GPIO, ADC, and PWM

## Key Features
- Automatic lid opening using IR sensing
- Bin fill-level detection using ultrasonic sensor
- Toxic gas detection and alerting
- Real-time status display on LCD
- Wireless notifications via ESP32 Wi-Fi

## Sensor Data Analysis
Sensor readings are post-processed in MATLAB to study usage patterns and dynamic behavior. Normalization and rate-of-change analysis are used to observe events such as bin usage and sudden state changes.

## Results
- Consistent lid actuation
- Reliable bin-full and gas detection
- Clear identification of usage events from sensor data

## How to Run
1. Flash the firmware using Arduino IDE
2. Connect hardware as per the block diagram
3. Power the ESP32
4. Observe output on LCD and serial monitor

## What I Learned
- Embedded system integration
- Real-time sensor handling
- State-machine based firmware design
- Hardware debugging and validation
- Basic signal analysis for sensor data

## Future Improvements
- RTOS-based task scheduling
- Power optimization and sleep modes
- Cloud-based monitoring dashboard
- Improved event classification
