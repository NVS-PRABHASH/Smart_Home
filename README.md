# Smart_Home
# ESP RainMaker + Manual Switch Control for 8 Relays Using ESP32  

 This project provides a seamless integration of manual and cloud-based control of up to 8 relays using the ESP32 microcontroller and ESP RainMaker platform. It enables real-time feedback and synchronization between physical switches and remote controls, ensuring reliable operation even without WiFi connectivity. This project is ideal for smart home automation, allowing control of lights, appliances, or other devices through ESP RainMaker or manual switches.

## Overview  
This project demonstrates how to control 8 relays using an ESP32 microcontroller, with both manual switches and cloud integration via the ESP RainMaker platform. The system provides real-time feedback, ensuring synchronization between physical switch operations and remote control, even in the absence of WiFi connectivity.

## Features  
- **Control Options**: Relays can be operated manually or through the ESP RainMaker app.  
- **Real-Time Feedback**: Updates relay state on the app and via physical switches in real time.  
- **No WiFi Mode**: Operate relays manually when WiFi is unavailable.  
- **Customizable**: Easy to adapt to different devices or configurations.  
- **Secure Provisioning**: Secure WiFi provisioning using BLE or SoftAP.  

## Components Required  
1. **ESP32 Development Board**  
2. **8-Channel Relay Module**  
3. **Manual Toggle Switches**  
4. **WiFi Network** (for ESP RainMaker functionality)  
5. **Jump Wires and Breadboard**  

## Wiring Diagram  
1. **Relay Connections**:  
   - Relay Pins: GPIO 23, 22, 21, 19, 18, 5, 25, 26  
   - Corresponding relays are controlled through these GPIOs.  

2. **Manual Switch Connections**:  
   - Switch Pins: GPIO 13, 12, 14, 27, 33, 32, 15, 4  
   - Switch states are read from these pins.  

3. **LED Indicators**:  
   - GPIO 2 for WiFi status.  

Refer to the code comments for additional pin configuration details.

## Software Requirements  
1. **Arduino IDE** (Configured for ESP32 development).  
   - Add ESP32 Boards Manager URL in Arduino Preferences:  
     `https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json`  

2. **ESP RainMaker Library** (Install via Arduino Library Manager).  

## Setup Instructions  
1. **Clone the Repository**  
   ```bash
   git clone https://github.com/yourusername/esp32-8-relay-rainmaker.git
   cd esp32-8-relay-rainmaker