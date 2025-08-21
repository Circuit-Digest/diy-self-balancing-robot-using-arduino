# DIY Self-Balancing Robot using Arduino
![Arduino UNO](https://img.shields.io/badge/Board-Arduino%20UNO-blue?logo=arduino)  ![Language](https://img.shields.io/badge/Language-C%2B%2B%2FArduino-yellow?logo=c%2B%2B) ![Component](https://img.shields.io/badge/Component-MPU6050%20%26%20L298N-green) 
![License](https://img.shields.io/badge/License-CircuitDigest-red)  
 
 

🔗 [DIY Self-Balancing Robot using Arduino](https://circuitdigest.com/microcontroller-projects/arduino-based-self-balancing-robot)  

📂 [Arduino Project](https://circuitdigest.com/arduino-projects)

---


---

![DIY Self-Balancing Robot using Arduino](https://circuitdigest.com/sites/default/files/projectimage_mic/DIY-Self-Balancing-Robot-using-Arduino.jpg)

---

## 🚀 Features
- Two-wheel self-balancing robot powered by **Arduino UNO**.  
- Uses **MPU6050 Gyroscope + Accelerometer** for orientation sensing.  
- Implements **PID algorithm** for real-time stability correction.  
- Controlled via **L298N motor driver** with geared DC motors.  
- Lightweight design powered by a **7.4V Li-ion battery**.  
- Fully 3D-printed chassis for durability and customization.  

---

## 🛠️ Hardware Requirements

| Component               | Quantity | Description |
|--------------------------|----------|-------------|
| Arduino UNO              | 1        | Main controller board |
| MPU6050                  | 1        | 6-axis accelerometer + gyroscope sensor |
| L298N Motor Driver       | 1        | Dual H-bridge motor driver |
| Geared DC Motors         | 2        | Yellow 12V DC gear motors |
| Wheels                   | 2        | Matched to DC motors |
| 7.4V Li-ion Battery      | 1        | Power source |
| 3D Printed Chassis       | 1        | Custom robot frame |
| Connecting Wires         | As req.  | For circuit connections |
| Nuts & Bolts             | As req.  | For motor & board mounting |

---

## ⚙️ How It Works
1. **Orientation Detection**: The MPU6050 continuously measures tilt (pitch and roll).  
2. **Data Processing**: Arduino reads sensor data via I²C and calculates the current angle.  
3. **PID Control**: The PID algorithm computes corrective motor actions based on tilt deviation.  
4. **Motor Control**: L298N motor driver receives PWM signals from Arduino to adjust motor direction and speed.  
5. **Balancing Act**:  
   - If robot leans forward → wheels move forward.  
   - If robot leans backward → wheels move backward.  
   - If balanced → motors stop.  

---

## 🔌 Circuit Connection

![Self-Balancing Robot Circuit Diagram](https://circuitdigest.com/sites/default/files/circuitdiagram_mic/Circuit-Diagram-for-DIY-Self-Balancing-Robot-using-Arduino.png)

### Arduino Pin Mapping
| Component Pin | Arduino Pin |
|---------------|-------------|
| MPU6050 Vcc   | 5V |
| MPU6050 GND   | GND |
| MPU6050 SCL   | A5 |
| MPU6050 SDA   | A4 |
| MPU6050 INT   | D2 |
| L298N IN1     | D6 |
| L298N IN2     | D9 |
| L298N IN3     | D10 |
| L298N IN4     | D11 |

---

## 🧠 Troubleshooting

| Issue | Possible Cause | Solution |
|-------|----------------|----------|
| Robot not balancing | Incorrect PID values | Re-tune Kp, Ki, Kd via Serial Monitor |
| Motors not running | Wrong motor driver wiring | Check IN1–IN4 connections |
| Robot works via USB but not battery | Power supply insufficient | Ensure 7.4V Li-ion can supply enough current |
| MPU6050 not detected | Loose I²C connections | Recheck SDA/SCL wiring |
| Robot keeps skidding | Poor wheel grip | Replace with better traction wheels |

---

## 📱 Applications
- Educational project for understanding **PID control systems**.  
- Foundation for **self-balancing scooters & robots**.  
- Robotics competitions and academic demonstrations.  
- Research prototype for **control system experiments**.  

---

## 🔮 Future Enhancements
- Add **Bluetooth/Wi-Fi module** for remote control.  
- Upgrade to **stepper motors** for smoother balance.  
- Use **better Li-Po batteries** for longer runtime.  
- Implement **mobile app interface** for PID tuning.  
- Expand to **ball-balancing robot** version.  

---

## 🧪 Technical Specifications

| Parameter | Value |
|-----------|-------|
| Controller | Arduino UNO (ATmega328P) |
| Sensor | MPU6050 (6-axis Gyroscope + Accelerometer) |
| Motor Driver | L298N Dual H-Bridge |
| Motors | 12V DC Geared Motors |
| Power Supply | 7.4V Li-ion Battery |
| Algorithm | PID Control |
| Communication | I²C for MPU6050, PWM for motors |

---

## 🔗 Links
- 📘 [DIY Self-Balancing Robot using Arduino](https://circuitdigest.com/microcontroller-projects/arduino-based-self-balancing-robot)  
- ⚡ [Arduino IDE Download](https://www.arduino.cc/en/software)  
- 📑 [Arduino Wire (I²C) Library Reference](https://www.arduino.cc/en/reference/wire)  
- 🔧 [L298N Motor Driver with Arduino](https://circuitdigest.com/microcontroller-projects/interfacing-l298n-motor-driver-with-arduino)  
- 🔧 [Arduino MPU6050 Sensor Module](https://circuitdigest.com/microcontroller-projects/interfacing-mpu6050-module-with-arduino)  
- 📂 [Arduino PID Library](https://github.com/br3ttb/Arduino-PID-Library)  
- 📂 [MPU6050 Arduino Library](https://github.com/jrowberg/i2cdevlib/tree/master/Arduino/MPU6050)  

---

## ⭐ Support
If you found this project useful, consider supporting CircuitDigest by exploring more tutorials and sharing this project with others.  

💡 *CircuitDigest – Open Source Electronics Projects & Tutorials for Makers, Engineers & Students.*  

---

## 🔖 Keywords
`Arduino UNO` `Self Balancing Robot` `MPU6050` `L298N Motor Driver` `PID Algorithm` `Arduino Project` `Gyroscope` `Accelerometer` `Two-Wheel Robot`
