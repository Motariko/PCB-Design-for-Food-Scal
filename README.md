# PCB-Design-for-Food-Scal: Custom PCB Design for Digital Food Scale

This repository contains the custom Printed Circuit Board (PCB) design for the ScalPro smart food scale project. The hardware is engineered to support precise weight measurement, user interaction via physical controls, and an integrated display system.

## Hardware Architecture and Schematic Design

The PCB design is centered around the ESP32 microcontroller, utilizing a dual-row header configuration for modularity and ease of maintenance. The circuit integrates several specialized subsystems to ensure reliable operation in a kitchen environment.

The Signal Acquisition Interface features a dedicated header for the HX711 Load Cell Amplifier, which is essential for high-resolution weight data acquisition with minimal signal interference. User input management is handled by multiple hot-swap tactile switches designed for primary functions such as Tare, Data Transmission, and System Sleep, providing a robust physical interface. Additionally, a standardized I2C LCD connector includes integrated voltage jumper points to allow for flexible power rail configuration across various display modules. The power distribution network is designed with dedicated input headers and battery management terminals to support portable operation via rechargeable battery cells.

## PCB Layout and Routing Specifications

The PCB was developed with a strict focus on signal integrity and power stability. The layout utilizes a single-layer routing strategy with widened power traces to minimize voltage drop and ensure consistent performance during high-current wireless transmissions, such as WiFi or Bluetooth operations.

Thermal and ground management is achieved through a large ground pour, which provides necessary electromagnetic interference shielding and effective heat dissipation for the onboard voltage regulators and the ESP32 module. The component placement is highly optimized to maintain a compact form factor, making it suitable for integration into a professional kitchen scale enclosure.

## Technical Summary

The main controller for this design is an ESP32 development board mounted via headers for serviceability. The board provides full hardware support for HX711 sensors, I2C liquid crystal displays, and Serial UART communication for debugging purposes. It supports dual-mode power input through either an external voltage source or an integrated battery system.

Developed by Aitsara Phetsila, Computer Engineering Student at Ramkhamhaeng University.
