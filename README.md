# Smart Baby Cradle Monitoring and Control System

## Overview
The **Smart Baby Cradle Monitoring and Control System** is an innovative IoT project built using a NodeMCU microcontroller. This system ensures the safety and comfort of a baby by monitoring environmental parameters, detecting crying, and providing remote control capabilities through a web application.

Key features include:
- Cry detection to alert caregivers.
- Temperature monitoring with automated fan/AC control.
- Remote control of the cradle's movement.
- Live video streaming via an integrated camera module.
- Real-time data storage and updates on a Firebase server.
- User-friendly web-based UI for monitoring and control.

## Features
1. **Cry Detection**:
   - Uses sound sensors to detect if the baby is crying.
   - Sends alerts to the web application in real time.

2. **Temperature Monitoring**:
   - Measures the temperature around the cradle using a temperature sensor.
   - If the temperature exceeds a set threshold, the system can automatically control a fan or AC via a remote interface.

3. **Cradle Control**:
   - Allows caregivers to control cradle movement remotely through the web UI.

4. **Camera Module Integration**:
   - Provides live video streaming of the baby’s activity directly in the web UI.

5. **Real-Time Data Sync**:
   - All sensor data (cry detection, temperature) is sent to a Firebase server.
   - The web application fetches and displays this data in real time.

## System Components
### Hardware
- **NodeMCU (ESP8266/ESP32)**: Microcontroller for IoT functionalities.
- **Microphone Module**: Detects crying sounds.
- **Temperature Sensor (e.g., DHT11/DS18B20)**: Measures ambient temperature.
- **Relay Module**: Controls fan/AC.
- **Motor Driver**: Drives cradle movement.
- **Camera Module (e.g., ESP32-CAM)**: Captures and streams live video.
- **Power Supply**: Powers the components.

### Software
- **NodeMCU Firmware**: Configures hardware functionality.
- **Firebase**: Stores and synchronizes data in real time.
- **Web Application**: Displays sensor data and provides control options.
- **Programming Languages**: C++ for NodeMCU and JavaScript/HTML/CSS for the web application.

## Installation and Setup
### Hardware Setup
1. Connect the microphone module to NodeMCU to detect sound.
2. Connect the temperature sensor to NodeMCU for temperature monitoring.
3. Attach the relay module for fan/AC control.
4. Connect the motor driver to control cradle movement.
5. Attach the camera module for live video streaming.
6. Ensure all components are powered appropriately.

### Software Setup
1. **NodeMCU Configuration**:
   - Use the Arduino IDE to write and upload the firmware to NodeMCU.
   - Include libraries for Firebase, DHT sensor, and any relevant motor control.

2. **Firebase Setup**:
   - Create a Firebase project and set up the Realtime Database.
   - Add the Firebase SDK credentials to the NodeMCU firmware.

3. **Web Application**:
   - Develop a web app to display real-time data (cry detection, temperature, video streaming) and provide control options.
   - Host the web app on Firebase Hosting or another hosting provider.

## Usage
1. Power on the system.
2. Access the web application through a browser.
3. Monitor live temperature, crying status, and video feed.
4. Use the controls in the web UI to:
   - Start/stop cradle movement.
   - Manually control fan/AC if needed.
5. Receive alerts for cry detection or abnormal temperature conditions.

## Project Dependencies
- Arduino IDE
- Firebase Realtime Database
- Libraries:
  - `Firebase ESP8266/ESP32`
  - `DHT` for temperature sensing
  - `ESP32-CAM` (if using ESP32 with a camera)

## Future Enhancements
- Add AI-based analysis for advanced cry detection and pattern recognition.
- Integrate voice commands for cradle control.
- Add mobile app support for greater accessibility.
- Implement battery backup for uninterrupted operation.

## Contributing
Contributions are welcome! Please feel free to submit issues or pull requests.

