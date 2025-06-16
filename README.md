# 🚨 IoT-Driven Motorcycle Accident Detection with Injury Severity and Location Tracking

An Internet of Things (IoT) based system designed to detect motorcycle accidents in real-time, evaluate injury severity using sensor data, and send emergency alerts with live GPS location to designated contacts and healthcare providers.

---

## 📌 Features

- ✅ Real-time accident detection
- 💥 Crash impact and tilt angle analysis
- ❤️ Heart rate monitoring (optional)
- 📍 Live GPS location tracking
- 📲 SMS alerts to emergency contacts using GSM
- ☁️ Optional cloud integration for real-time data storage and monitoring

---



## 🚧 Project Overview

Motorcycle accidents are highly fatal due to the lack of external protection and delayed emergency responses. This project aims to provide a low-cost, effective accident detection system using IoT devices. The system analyzes sensor data from the motorcycle and rider to detect crashes, assess injury severity, and send alerts with location coordinates for rapid assistance.

---

## 🧠 System Architecture
Rider/Bike

[MPU6050 - Gyro & Accelerometer]

[Microcontroller (Arduino/ESP32)]
── [GPS Module - Location]
── [GSM Module - SMS]
── [Heart Rate Sensor - Optional]

[Alert System → Emergency Contacts]


---

## 🔌 Hardware Components

| Component                | Description                    |
|--------------------------|--------------------------------|
| Arduino Uno / ESP32      | Main microcontroller unit      |
| MPU6050                  | Accelerometer + Gyroscope      |
| NEO-6M GPS Module        | For real-time GPS tracking     |
| SIM800L GSM Module       | For sending SMS alerts         |
| Heartbeat Sensor (opt)   | For rider health data          |
| Li-ion Battery/PowerBank | Power supply                   |
| Jumper wires, breadboard | Prototyping accessories        |

---

## 💻 Software Requirements

- Arduino IDE
- Embedded C/C++
- SIM card with SMS balance
- Firebase/ThingSpeak (Optional cloud)
- MIT App Inventor / Android Studio (for mobile app, optional)

---

## ⚙️ Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/accident-detection-iot.git
   cd accident-detection-iot

Open the .ino file in Arduino IDE

Install required libraries:

TinyGPS++

SoftwareSerial

Wire (default for MPU6050)

Upload the code to your Arduino or ESP32 board

Connect hardware components as per the schematic in /hardware_diagram/

Insert SIM card and ensure GSM and GPS modules are powered

▶️ How It Works
Impact Detection: MPU6050 detects sudden fall/impact based on threshold values.

Injury Severity: Estimated based on force and orientation angles.

GPS Location: Captured using the NEO-6M module.

Alert: GSM module sends an SMS with Google Maps link to emergency contacts.

