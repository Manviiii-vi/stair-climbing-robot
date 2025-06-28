# 🧠 System Design – Stair Climbing Robot

> This document outlines the system architecture and working logic of the stair-climbing robot.

---

## 🔧 Core Components & Architecture

### 📟 Microcontroller
- **ESP32**
  - Controls all motors (BO and N20)
  - Runs motor control logic and coordination
  - Can support future features like Wi-Fi/Bluetooth

### ⚙️ Actuation
- **N20 Motors** — responsible for vertical lift via rack & pinion
- **BO Motors** — responsible for forward motion and base movement
- **L298N Motor Driver** — handles direction and power switching

---

## ⚙️ Mechanical Design

- **Base Platform** made with MDF
- **Pulley and Rack & Pinion Mechanism** for step climbing
- **Lead Screws with threaded rods** — allows lift to occur in sync
- Center of gravity maintained to ensure balance on step edges

---

## 🔌 Power Supply

- Powered by a rechargeable battery pack
- Connected to ESP32 and motor driver
- Voltage regulation ensures no overheating or power loss

---

## 🔁 Workflow (How It Climbs Stairs)

1. **Forward Motion**
   - BO motors move the robot forward to the base of a stair.

2. **Stair Detection (manual in v1)**
   - In future: IR/ultrasonic sensor detects stair edge.

3. **Lift Activation**
   - N20 motors lift front section via rack & pinion.
   - Once the front is placed on the next stair, rear is pulled up.

4. **Repetition**
   - Steps 1–3 are repeated until stair set is climbed.

---

## 🔮 Future System Expansion

- **Sensors**:
  - IR or ultrasonic for step detection
  - Gyroscope for balance and tilt detection

- **Communication**:
  - Bluetooth or Wi-Fi app control (using ESP32)
  - OTA updates and remote monitoring

- **Smart Control**:
  - AI/ML-based terrain detection and adaptive motion

---

## 🛠️ Development Tools

| Tool        | Purpose                            |
|-------------|-------------------------------------|
| ESP-IDF / Arduino Core for ESP32 | Programming ESP32 microcontroller |
| GitHub      | Version control, teamwork           |
| Fritzing    | (Planned) Circuit diagrams          |
| Draw.io     | Flowcharts & architecture           |

---

> File maintained by: Manvi  
> Last updated: June 2025









