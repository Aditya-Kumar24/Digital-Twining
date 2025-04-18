# 🚗 Digital Twin 4WD Mobility Car Project

This project showcases a real-time **Digital Twin** implementation of a 4WD mobility prototype using **ESP32-CAM**, **Arduino R4**, and a **Unity-based simulation environment**. It aims to bridge the gap between hardware and software using live telemetry, video streaming, and synchronized simulation.

---

## 🔧 Features

### ✅ Hardware Components
- 4WD Robotic Car Chassis
- ESP32-CAM (for live video streaming)
- Arduino UNO R4 (central controller)
- Ultrasonic Sensor (obstacle detection)
- Motor Driver Module (L298N)
- Power Supply Module
- IR Sensors (for line following, optional)

### 🖥️ Software Components
- **Unity**: Simulated environment for the digital twin
- **Arduino IDE**: Embedded programming
- **ESP32-CAM**: Real-time video stream over Wi-Fi
- **WebSocket/MQTT**: Communication protocol (for Unity ↔ ESP32)
- **Cloud Logging**: Firebase / Google Sheets (optional)
- **Telemetry Dashboard**: Visual display of data like speed, direction, battery, and obstacle distance

---

## 🧠 Core Functionalities

- 🔄 **Real-Time Synchronization** between the physical and virtual car
- 📷 **Live Streaming** from the ESP32-CAM to your local network or cloud
- 🚧 **Obstacle Detection** using ultrasonic sensors
- 📊 **Telemetry Data** sent to Unity dashboard & cloud database
- 🧭 **Remote Navigation** through UI in Unity or mobile controller
- 🌐 **Digital Twin Dashboard** for control, simulation, and data logging

