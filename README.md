# Self-Parking Car

An autonomous car prototype capable of identifying parking spaces and performing self-parking maneuvers using various sensors, actuators, and an STM32 microcontroller.  
This project showcases basic robotics, control systems, and embedded programming applied to autonomous driving.
![image](https://github.com/user-attachments/assets/b8eb420d-4c0f-44c4-a4ec-5bb96f19fa06)

---

##  Hardware Used

- **Microcontroller**: STM32F401-RE  
- **Ultrasonic Sensors**: 3x HC-SR04  
  - Front, rear, and side sensors  
  - All use Timer 1 in base time mode  
- **Servo Motor**: DMS-MG90-A (270º rotation)  
  - PWM: Timer 3, Channel 4  
  - Control pin: PC9  
- **DC Motor**: JCA25370  
  - Max voltage: 12V  
  - Max speed: 370 RPM  
  - Integrated encoder: 270 pulses per revolution  
  - PWM: Timer 4, Channel 3  
  - Control pins: PB8, PC9  
  - Encoder input: Timer 2 via PA0 and PA1  

---

##  Program Logic

1. The ultrasonic sensors detect distance to obstacles.
2. The STM32 processes sensor data to evaluate if a parking space is available.
3. When a suitable space is detected, it performs the parking maneuver autonomously.
4. Real-time control of the servo and motor is managed using timers and feedback from the encoder.

---

##  Flowchart
![image](https://github.com/user-attachments/assets/17c7dc88-03f1-430e-a326-acf293e3ce6a)

---

##  Demo Video

https://youtube.com/shorts/lFJc5HF0pDM

---

## 📁 Project Structure


