# 🔧 AI-Powered Raspberry Pi 4B Smart 4WD Rover

This project presents a fully autonomous 4WD robotic vehicle, powered by a **Raspberry Pi 4B**, equipped with **AI-based object detection**, **real-time obstacle avoidance**, **metal detection**, and **infrared (IR) vision**, all controllable via a **mobile interface** through Wi-Fi and Bluetooth.

Developed as part of my **2nd Semester Digital Logic Design (DLD) Project**, this rover combines embedded systems, computer vision, and sensor fusion into a modular and extensible smart system.

---

## 🚀 Features

- ✅ **Mobile-Controlled 4WD** via Bluetooth/Wi-Fi Hotspot
- 🧠 **Object Detection** using OpenCV + MobileNetSSD
- 🛑 **Obstacle Avoidance** using Ultrasonic sensors with auto-stop under 6cm at full speed
- 🧲 **Underground Metal Detection** using analog sensors (via SPI)
- 🔁 **360° Environmental Scanning** with rotating servo-mounted sensors
- 📷 **IR Camera Streaming** in real-time via Thonny terminal
- 🧵 **Multithreaded Processing** for independent module operations
- 📲 **Mobile Interface** for live feedback and control signals

---

## 🧱 System Architecture

- **Microcontroller**: Raspberry Pi 4B (4GB)
- **Programming Language**: Python 3
- **IDE**: Thonny (Raspberry Pi OS)
- **Modules**:
  - `motor_control.py` – movement control
  - `ultrasonic_sensor.py` – distance measurement
  - `metal_detector.py` – SPI-based analog read
  - `infrared_camera.py` – real-time video stream
  - `object_detection.py` – OpenCV AI detection
  - `avoidance_system.py` – logic for dynamic obstacle handling
  - `main.py` – orchestrator module using threading

---

## 🛠️ Hardware Components

- Raspberry Pi 4B (with Raspbian OS)
- L298N Motor Driver
- IR Camera (Night Vision Compatible)
- Ultrasonic Sensors (x2)
- Servo Motor Module
- Analog Metal Detection Sensor
- 4 Geared Motors + Wheels (4WD Chassis)
- Battery Pack (12V)
- Jumper Wires, Breadboard, Mounts

---

## ⚙️ Installation

sudo apt update && sudo apt upgrade
sudo apt install python3-opencv python3-pip
pip install RPi.GPIO spidev bash
📁 Place deploy.prototxt and mobilenet_iter_73000.caffemodel in the root directory for object detection to function.

---

## ▶️ Running the Rover

bash
Copy
Edit
python3 main.py
This launches all modules (camera, object detection, obstacle avoidance) in parallel using multithreading.

---

## 📡 Application & Use Cases

Originally created for underground metal and mineral detection, this platform has real-world applications in:

### 🚨 Disaster Search and Rescue (via AI + terrain sensing)

### 🌍 Geological Surveying

### 🌱 Smart Agriculture (mapping soil mineral content)

### 🔐 Surveillance Bots

---

## 📈 Project Outcomes

- Mastery of GPIO, SPI communication, and sensor interfacing
- AI-Computer Vision deployment on embedded hardware
- Modular design to enable rapid experimentation and extension
- Real-time edge computing capabilities

## 👤 Author

Ubaid ur Rehman
Computer Science Undergraduate – NUST
Semester 2 – Digital Logic Design Final Project

Feel free to contribute, raise issues, or collaborate on improvements!
