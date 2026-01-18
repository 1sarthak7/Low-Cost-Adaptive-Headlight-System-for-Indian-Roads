# Low-Cost-Adaptive-Headlight-System-for-Indian-Roads
# SMARTBEAM-LITE 🚗💡  
### An Affordable Adaptive Headlight System for Indian Roads

SMARTBEAM-LITE is a **low-cost, intelligent adaptive headlight prototype** designed to reduce night-time glare caused by improper use of high-beam headlights on Indian roads.  
The system demonstrates how **selective beam control**—similar in concept to luxury Matrix LED systems—can be achieved using **affordable hardware and computer vision**.

---

## 🧠 Problem Statement

Night-time driving on Indian roads is unsafe due to the widespread and continuous use of high-beam headlights by cars, trucks, and buses.  
This causes glare-induced temporary blindness, eye strain, and increases the risk of road accidents.

While premium vehicles offer adaptive or matrix LED headlights, these systems are:
- Expensive  
- Limited to luxury cars  
- Not accessible to most Indian drivers  

There is a need for a **cost-effective, scalable, and practical solution** tailored for Indian road conditions.

---

## 💡 Proposed Solution

SMARTBEAM-LITE is a **technology demonstrator** that uses:
- **Camera-based perception (webcam + laptop processing)**
- **Embedded hardware execution (NodeMCU)**
- **Segmented LED beam control**

The system detects oncoming vehicle headlights and selectively turns OFF specific LED segments to prevent glare, while keeping the rest of the road illuminated.

---

## 🏗️ System Architecture

**Perception Layer (Laptop)**
- Webcam captures road view
- Computer vision algorithm detects bright headlight regions
- Determines glare position (Left / Center / Right)

**Control Layer (NodeMCU)**
- Receives commands from laptop via Serial/Wi-Fi
- Controls multiple LED segments
- Simulates adaptive beam shaping

---

## 🔧 Hardware Components

- NodeMCU (ESP8266)
- 5–10 High-brightness LEDs (segmented beam)
- Resistors & breadboard
- USB power supply
- Webcam (for perception)
- Laptop (for processing)

---

## 🧪 Software Stack

- Python 3
- OpenCV (for image processing)
- Serial / Wi-Fi communication
- Arduino IDE (NodeMCU firmware)

---

## ⚙️ Working Principle

1. Webcam captures live road video
2. Laptop processes frames to detect bright glare regions
3. Frame is divided into zones (Left / Center / Right)
4. Decision command is sent to NodeMCU
5. Corresponding LED segments are turned OFF
6. LEDs return to normal once glare is gone

---

## 🎯 Key Features

- Selective glare blocking (not full beam dip)
- Low-cost and modular design
- Real-time response
- Demonstrates feasibility of adaptive headlights
- Designed for Indian traffic behavior

---

## 🧠 Design Thinking Approach

- **Empathize:** Understand driver discomfort and accident risk due to glare  
- **Define:** Excessive high-beam usage without adaptive control  
- **Ideate:** Affordable alternative to luxury matrix headlights  
- **Prototype:** Hardware + software working model  
- **Test:** Multiple lighting conditions and angles  

---

## 🚀 Why This Project Matters

- Improves night-driving safety
- Addresses a real and common Indian road problem
- Bridges the gap between luxury automotive tech and mass-market needs
- Demonstrates hardware–software co-design

---

## ⚠️ Disclaimer

This project is a **prototype and technology demonstrator** created for academic and exhibition purposes.  
It is **not intended for direct deployment in vehicles** without further automotive-grade testing and certification.

---

## 📌 Future Improvements

- Embedded vision using ESP32-CAM
- Smarter glare classification using ML
- Integration with real vehicle headlight assemblies
- Weather and fog adaptation

---

## 👤 Author

**Sarthak Bhopale**  
Engineering Student | Developer  
Project created as part of **Design Thinking – II**

---

## 📜 License

This project is open-source and available for educational and research purposes.
