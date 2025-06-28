# 🔁 Control Logic – Stair Climbing Robot

> This document explains the basic control logic behind the movement and lift mechanisms of the robot.

---

## 🧠 High-Level Overview

The robot operates in a loop of detecting stairs, moving forward, lifting the front section, and then pulling up the rear section. It uses two types of motors:

- **BO Motors** – for base movement (forward/backward)
- **N20 Motors** – for vertical lift using a rack and pinion + pulley mechanism

Controlled by an **ESP32 microcontroller** via **L298N motor drivers**.

---

## ⚙️ Step-by-Step Logic Flow

### 1. Forward Movement
- Robot moves forward using BO motors until it reaches a stair (manual or future sensor trigger).
- Controlled via digital HIGH/LOW signals to L298N motor driver.

### 2. Stop at Stair Edge
- Robot halts when it reaches the edge (currently timed/manual; future: IR/Ultrasonic sensor).

### 3. Front Lift
- N20 motors are activated to raise the front part using the rack and pinion mechanism.
- Lift is time-based or can be tied to a limit switch in the future.

### 4. Rear Pull-Up
- After the front is placed on the next step, the base (rear) is lifted by continuing motor rotation.

### 5. Repeat Cycle
- Once level, robot moves forward to the next stair and repeats.

---

## 🧪 Testing Notes
- Initial testing will use `delay()` for timing the motor operation.
- PWM control via `analogWrite()` will be tuned for each motor.
- Sensor integration planned in v2.

---

## ⏳ Future Improvements
- Use sensors for stair detection and edge alignment
- Replace delay-based logic with encoder-based or feedback control
- Add gyroscope or accelerometer for tilt management

---

> Maintained by: Manvi  
> Created: June 2025
