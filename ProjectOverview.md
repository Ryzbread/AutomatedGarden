**Project Overview**

* Goal: Design and implement a solar-powered garden automation system with three separate watering zones, each controlled by a dedicated node.
* Key features:
        + Soil moisture sensors to monitor soil conditions
        + WiFi connectivity for communication between nodes and the main controller
        + Solar power for each node and main controller
        + Solenoid valves for precise water control
        + Main controller with user interface (UI) for monitoring and controlling the system

**System Components**

1. **Main Controller**:
        * ESP32 or ESP8266 board for main controller
        * WiFi module (e.g., ESP01S) for communication between nodes and main controller
        * Battery backup (car battery) to ensure power supply during night hours
        * Solar panel array with charge controller for recharging batteries
        * User interface (UI) for monitoring and controlling the system
2. **Measuring Nodes**:
        * ESP-01S board for each measuring node
        * WiFi connectivity for communication between nodes and main controller
        * Soil moisture sensors to monitor soil conditions
        * No battery power, only solar power.
3. **Watering Zone Nodes**:
        * ESP-01S board for each watering zone node
        * WiFi connectivity for communication between nodes and main controller
        * Solenoid valves for precise water control
        * No battery power, only solar power.

**System Functionality**

1. **Node Communication**:
        * Each measuring node communicates with the main controller via WiFi
        * Main controller polls soil moisture data from each measuring node and determines water control needs
2. **Water Control**:
        * Solenoid valves controlled by main controller based on soil moisture readings
        * Precise water control to prevent over-watering or under-watering
3. **Power Management**:
        * Solar panels recharge batteries during day hours
        * Deep cycle batteries store energy for night hours
