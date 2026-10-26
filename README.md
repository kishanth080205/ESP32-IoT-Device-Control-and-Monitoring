
# ESP32 IoT Device Control and Monitoring

## Project Overview
ESP32-based IoT project for wireless LED control using Wi-Fi, MQTT, Android applications and Bluetooth, with DHT11 sensor data monitoring.
This project was carried out during my internship at CDAC Chennai from June 6, 2025, to July 11, 2025. It focuses on developing an IoT-based system to control an ESP32 development board's onboard LED wirelessly using Wi-Fi, mobile applications, MQTT, and Bluetooth communication.

The project also covers interfacing the ESP32 with a DHT11 temperature and humidity sensor and sending sensor data to a dashboard for visualization.

## Objectives
- Control the ESP32 onboard LED remotely using Wi-Fi.
- Develop a mobile interface for LED ON/OFF operations.
- Implement MQTT-based communication between the ESP32 and a mobile application.
- Explore Classic Bluetooth and Bluetooth Low Energy (BLE) communication.
- Interface a DHT11 sensor with the ESP32 for temperature and humidity monitoring.
- Explore cloud-based data visualization platforms for IoT monitoring.

## Hardware Components
- ESP32 Development Board
- DHT11 Temperature and Humidity Sensor
- USB Cable for programming and power
- Breadboard and jumper wires
- Android smartphone for mobile control and testing

## Technologies and Tools
- **Programming:** Arduino C/C++ and Kotlin
- **Embedded Development:** Arduino IDE and ESP32 board support package
- **Mobile Applications:** MIT App Inventor, IoT MQTT Panel, Blynk IoT
- **Communication Protocols:** Wi-Fi, HTTP, MQTT, Classic Bluetooth and BLE
- **MQTT Library:** PubSubClient
- **MQTT Broker:** Mosquitto test broker, as configured in the report
- **Sensor:** DHT11
- **Data Visualization Platforms Explored:** Firebase Realtime Database, ThingSpeak and RemoteXY

## Project Modules

### 1. Wi-Fi-Based LED Control
Programmed the ESP32 to connect to a Wi-Fi network and run an HTTP web server. LED ON/OFF commands are sent through HTTP requests, which the ESP32 processes to control the onboard LED.

### 2. Android Application Development
Developed an Android application using Kotlin with separate LED ON and LED OFF buttons. The application sends HTTP requests to the ESP32 to control the LED.

### 3. MIT App Inventor Integration
Designed a simple mobile interface using MIT App Inventor to send commands to the ESP32 over Wi-Fi.

### 4. MQTT-Based LED Control
Configured the ESP32 to communicate with an MQTT broker using the PubSubClient library. The IoT MQTT Panel application sends ON/OFF messages to the `esp32/led` topic, which the ESP32 subscribes to and processes.

### 5. Bluetooth Communication
Explored Classic Bluetooth and BLE communication with the ESP32 using mobile testing applications, including Serial Bluetooth Terminal and nRF Connect.

### 6. Temperature and Humidity Monitoring
Worked on interfacing the ESP32 with a DHT11 sensor and exploring ways to transmit sensor readings to a data visualization dashboard.

## Working Principle
1. The ESP32 is powered and programmed through the Arduino IDE.
2. The board establishes a wireless connection using Wi-Fi or Bluetooth, depending on the selected communication method.
3. The mobile application sends commands using HTTP or MQTT, or communicates through Bluetooth.
4. The ESP32 processes the received commands and switches the onboard LED ON or OFF.
5. For sensor monitoring, the DHT11 provides temperature and humidity readings that can be transmitted to a suitable visualization platform.

## Results
- Demonstrated Wi-Fi-based remote control of the ESP32 onboard LED.
- Implemented HTTP request handling for LED ON/OFF operations.
- Configured MQTT communication for receiving LED control commands.
- Explored mobile application integration and Bluetooth connectivity.
- Worked on DHT11 sensor interfacing and dashboard-based data visualization.

## Applications
- Smart home automation
- Wireless device control
- IoT prototyping and experimentation
- Remote monitoring systems
- Sensor-based environmental monitoring

## Internship
**Organization:** Centre for Development of Advanced Computing (C-DAC), Chennai  
**Duration:** June 6, 2025 – July 11, 2025

## Author
HB. Kishanth

*Note: The repository should contain the actual source code and setup instructions for the modules you implemented. Include only platforms and features that you can demonstrate or substantiate with your code and results.*
