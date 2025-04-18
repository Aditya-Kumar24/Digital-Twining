Digital Twin Smart Car System

This project integrates Unity, Arduino UNO R4 WiFi, and ESP32-CAM into a unified system where a physical and digital car synchronize to follow a target and avoid obstacles in real time.

📅 Overview

The project is composed of three main components:

Unity Game Engine: Simulates a digital twin car following a target using waypoints and NavMesh.

Arduino UNO R4 WiFi: Controls a 4WD real robotic car using L298N Motor Driver.

ESP32-CAM: Detects obstacles in front of the real car and notifies Unity.

📊 Components Used

Component

Role

Unity Engine

Simulation and command center

Arduino UNO R4 WiFi

Motor control via HTTP

ESP32-CAM

Obstacle detection via camera

L298N Motor Driver

Drives motors

DC Motors (4x)

Physical car movement

WiFi Router

Local communication bridge

🚀 Unity Code Components

1. CarController.cs

Handles physics-based car control and optional auto-drive logic.

2. PathFollower.cs

Moves the car along waypoints or toward a target while handling pathfinding and orientation.

3. CarFollower.cs

Sends HTTP movement commands (forward, left, right, stop) to the Arduino based on Unity's car position vs. the target.

4. PlayerNavMesh.cs (Optional)

Used if employing NavMesh for navigation.

Network Communication

From

To

Method

Purpose

Unity

Arduino

HTTP

Move commands (/forward)

ESP32-CAM

Unity

HTTP

Notify of obstacle

🌐 Setup Flow

Upload ESP32-CAM and Arduino sketches with proper SSID/passwords.

Connect all devices to same WiFi network.

Set the Arduino IP in CarFollower.cs in Unity.

Setup target object and car prefab in Unity.

Press Play: Car starts to follow target.

ESP32 will detect obstacles and notify Unity. Unity updates obstacle in scene and instructs car to avoid.

📄 To Do

Improve ESP32-CAM ML model for better detection.

Implement Unity HTTP server for 2-way sync.

Add battery and voltage management for real car.

💼 Credits

Developed for a hackathon/robotics automation project. Using ESP32, Arduino UNO R4 WiFi, Unity 3D.

