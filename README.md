# Smart-Traffic-and-Accident-Management
AI-based intelligent traffic management system which dynamically controls traffic signals.   Uses real-time video analysis with deep learning.   Automatically detects:   Emergency vehicles   Road accidents and provides alert to nearby hospitals.   Traffic density

# AI-Based Intelligent Traffic Management System 🚦

An AI-driven traffic management system that uses real-time computer vision and deep learning to detect emergency vehicles, road accidents, and traffic density, enabling dynamic traffic signal control and faster emergency response.

---

## 📌 Problem Statement

Traditional traffic signal systems operate on fixed timing and lack real-time adaptability. As a result:
- Emergency vehicles like ambulances get stuck in traffic
- Road accidents are not detected or reported instantly
- Manual traffic control is slow and inefficient
- Traffic congestion is poorly managed during peak hours

These limitations lead to delayed emergency response, increased accident risks, and inefficient traffic flow.

---

## 💡 Proposed Solution

This project proposes a **fully automated AI-based Intelligent Traffic Management System** that:
- Analyzes live or recorded traffic video feeds
- Detects emergency vehicles and road accidents in real time
- Estimates lane-wise traffic density
- Dynamically controls traffic signals using Arduino
- Automatically sends emergency alerts with GPS location to nearby hospitals

The system integrates **deep learning, computer vision, embedded hardware, and communication modules** to provide a scalable smart-city-ready solution.

---

## ⚙️ System Architecture (High Level)

- **Traffic Camera** → Captures live video feed  
- **AI Processing Unit (Python)**  
  - Emergency Vehicle Detection (YOLO – `best.pt`)
  - Accident Detection (`latestAccident.pt`)
  - Traffic Density Estimation (YOLOv8 – `yolov8n.pt`)
  - Central Decision-Making Engine (Priority Based)
- **Serial Communication** → Python to Arduino
- **Arduino Microcontroller** → Controls traffic signals
- **GSM + GPS Modules** → Sends emergency alerts

---

## 🧠 Key Features

- Real-time traffic monitoring using computer vision  
- AI-based ambulance and fire truck detection  
- Custom-trained YOLO model for accurate local ambulance detection  
- Automatic green corridor creation for emergency vehicles  
- Real-time road accident detection  
- Immediate traffic halt during accidents  
- GSM + GPS based emergency alerts to hospitals  
- Lane-wise traffic density estimation  
- Adaptive traffic signal timing (no fixed cycles)  
- Priority-based traffic control:  
  **Accident > Emergency Vehicle > Normal Traffic**  

---

## 🛠️ Technologies Used

### AI & Computer Vision
- Python
- YOLO (Ultralytics)
- OpenCV
- TensorFlow / PyTorch (model training)

### Hardware
- Arduino Uno
- Traffic signal LEDs (Red, Yellow, Green)
- GSM Module
- GPS Module

---

## 📂 Project Structure
