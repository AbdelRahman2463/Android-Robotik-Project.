🤖 Android Robotik Project

An Android-controlled robotic system that combines manual joystick control with autonomous object detection and tracking — built to demonstrate the integration of mobile development, embedded systems, and computer vision.

Project for the University of Applied Sciences Bonn-Rhein-Sieg.

📖 Overview

The system utilizes an Android Smartphone mounted on a robot platform powered by an STM32 Microcontroller. It supports two primary modes of operation:

Mode
Description
Technology
Manual Control
Real-time robot navigation via a virtual joystick interface
Bluetooth Serial
Autonomous Tracking
Automatic object following (Line or Ball) using the phone's camera
CameraX + Computer Vision




The Android application serves as the central hub, processing live video feed at ~30 FPS to calculate movement errors and sending proportional control commands to the STM32 via Bluetooth. The system includes safety mechanisms to stop the robot if the connection is lost or the target is no longer detected.

🛠️ Hardware

•
STM32 Microcontroller — Main controller for motor PWM and Bluetooth communication.

•
Bluetooth Module — Wireless data transfer between the app and the robot.

•
Motor Driver — Controls DC motor direction and speed.

•
Android Smartphone — Provides UI, Bluetooth connectivity, and camera-based tracking.

•
DC Motors & Chassis — Mechanical and power components for movement.

⚙️ Setup

1.
Clone the repository:

Bash


git clone https://github.com/AbdelRahman2463/Android-Robotik-Project.git
cd Android-Robotik-Project





2.
Open in Android Studio:

•
Launch Android Studio and select Open.

•
Navigate to the Android-Robotik-Project folder and select it.

•
Wait for Gradle to sync and download dependencies.



3.
Build and Run:

•
Connect your Android device (ensure Developer Options and USB Debugging are enabled ).

•
Click the Run button (green play icon) in Android Studio.



📁 Project Structure

Plain Text


android-robotik-project/
├── app/
│   ├── src/main/
│   │   ├── java/com/hbrs/
│   │   │   ├── MainActivity.java      # Central coordinator & UI logic
│   │   │   ├── Bluetooth/             # Bluetooth device discovery
│   │   │   └── ORB/                   # Robot control interface
│   │   └── AndroidManifest.xml        # Permissions (Camera, Bluetooth)
│   └── build.gradle                   # App dependencies & configuration
├── docs/
│   └── FinalReport.pdf                # Full project documentation
├── README.md                          # Project overview
├── LICENSE.md                         # MIT License
└── .gitignore                         # Git exclusion rules



📊 Results

The system achieves smooth real-time operation with a response latency of approximately 33ms. The use of the HSV color space for ball detection provides robustness under variable lighting conditions. Testing confirmed reliable transition between manual and autonomous modes, with failsafe callbacks ensuring stable operation.

👥 Authors

•
Abdelrhman Aldwary (9058915)

•
Abdallah Alqudah (9058873)

•
Haya Bawati (9058924)

Supervised by Prof. Thomas Breuer — University of Applied Sciences Bonn-Rhein-Sieg, 2026.

📄 Full Report

See docs/FinalReport.pdf for the complete project report and technical specifications.

