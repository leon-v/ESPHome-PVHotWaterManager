# Hot Water Cylinder Controller

This project utilizes an ESP32 microcontroller to control a hot water cylinder, providing functionalities such as monitoring power consumption, managing runtime, setting temperature limits, intelligently utilizing PV power, optimizing energy costs, and minimizing losses by strategic energy addition. Below is a breakdown of the components and functionalities:

## Components:

- **ESP32 Microcontroller**: Utilizes the ESP32-S2-Saola-1 board.
- **Current Clamp Sensor (CT Clamp)**: Monitors AC current consumption.
- **Status LED**: Indicates the status of the device.
- **Temperature Setting Switch**: Controls the temperature setting of the cylinder.

## Functionalities:

1. **Power Monitoring**: Utilizes a CT clamp sensor and an ADC to measure power consumption accurately.
2. **Energy Tracking**: Tracks total daily energy consumption in kWh.
3. **Runtime Management**: Manages the runtime of the system, including calculating runtime remaining and estimating catchup time.
4. **Energy Limiting**: Allows setting energy limits for the hot water cylinder.
5. **Intelligent Energy Usage**: Utilizes PV power efficiently and adds more heat until 7 am when more expensive energy starts.
6. **Loss Optimization**: Minimizes losses by strategically adding energy late.
7. **Home Assistant Integration**: Provides an API for integration with Home Assistant.
8. **Over-the-Air (OTA) Updates**: Supports OTA updates for firmware.

## Configuration:

- **WiFi**: Connects to the configured WiFi network for internet connectivity.
- **Time Synchronization**: Syncs the device's time using SNTP.
- **Logger**: Enables logging for debugging purposes.
- **UART Configuration**: Configures UART for communication with relay control.

## Installation:

Follow the usual ESPHome process you use.

---

**Note**: Ensure proper safety precautions and consult with professionals for electrical installations.
