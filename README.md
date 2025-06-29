# Stair Climbing Robot

> A project to design and develop a robot capable of autonomously climbing stairs, overcoming the limitations of traditional wheeled robots on uneven terrains.

![Project Demo](https://img.youtube.com/vi/sHyekTDxaH8/0.jpg)

[Watch the Project Demo Video](https://youtu.be/sHyekTDxaH8?si=n2f1cvXuMfX4rgW8)

---

## 🔍 Problem Statement
Traditional wheeled robots face limitations in navigating uneven terrains like staircases. Our goal is to develop a stair-climbing robot capable of ascending and descending stairs autonomously, offering improved mobility for robotics applications in domestic, industrial, and emergency environments.

---

## 👥 Team Members
- **Mentor:** Ashutosh Sahu
- **Yash Gupta** – Hardware
- **Manvi** – Software
- **Himanshu Prasad** – Software

---

## 🧠 Inspiration
This robot is inspired by mechanical solutions demonstrated in the video ["Stair Climbing Robot"](https://youtu.be/sHyekTDxaH8?si=n2f1cvXuMfX4rgW8).

---

## 🚀 Project Description
This project focuses on designing and building a robot that uses a unique mechanical structure and motorized lift system to move up and down stairs. The robot uses an ESP32 microcontroller to receive commands and drive the motors, combined with a rack and pinion mechanism to achieve elevation. It is compact, cost-effective, and built using commonly available components.

---

## 📌 Features
- Autonomous stair detection and movement
- Climbing via mechanical rack and pinion + pulley system
- Controlled by ESP32 for efficient motor handling
- Portable, affordable, and replicable

---

## 🧩 Technologies & Hardware Used

### 🔧 Hardware:
- ESP32 microcontroller
- L298N Motor Driver Module
- N20 Motors
- BO Motors and Wheels
- Rack and Pinion Mechanism
- Pulley System
- Lead Screw with Threaded Rods
- MDF (Wooden Cardboard)
- Battery Pack
- Jumper Wires, Proto Board

### 💻 Software & Tools:
- Arduino IDE (ESP32 Programming)
- Embedded C/C++
- GitHub (Version control & collaboration)

---

## ⚙️ How It Works
The robot uses a **pulley-driven rack and pinion** mechanism to lift itself step-by-step. The ESP32 controls the N20 and BO motors via the L298N motor driver. The motors rotate the threaded rods and pulleys, allowing the robot to lift its front or rear depending on its position on the stairs. It detects the stair edge, stops, and then activates the climb mechanism. Coordination between motors ensures balance and stability.

---

## 📷 Media
Photos, progress shots, and final build images will be uploaded in the `images/` folder.
You can also check out the video demonstration linked above for a working overview.

> Images will showcase internal structure, wiring, and step-by-step construction of the robot.

---

## 📈 Future Plans
- Add ultrasonic or IR sensors for dynamic obstacle detection
- Implement Bluetooth/Wi-Fi control via mobile app
- Optimize weight and structure with 3D-printed parts
- Use machine learning for terrain adaptation

---

## 📁 Folder Structure 
```
stair-climbing-robot/
├── code/
├── images/
├── hardware/
├── docs/
├──idea/
├── README.md
```

---

## 📜 License
MIT License

---

## 🌟 Stay Tuned
We will keep updating this repository with:
- Circuit diagrams
- Arduino/ESP32 code
- Photos & videos of the build
- Instructions to replicate

> ⭐ Star this repo to stay updated!
