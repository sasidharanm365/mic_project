# mic_project
# 🔐 Adaptive Time-Locked Wireless Charging Station

## 📌 Project Overview

The **Adaptive Time-Locked Wireless Charging Station** is an embedded system designed to provide secure and time-controlled wireless charging for smartphones in public places such as colleges, libraries, airports, shopping malls, railway stations, and offices.

The system combines wireless charging, phone detection, password-based authentication, automatic locking, and timer-controlled charging using an ESP8266 NodeMCU.

Users can place their smartphones inside the charging compartment, enter a charging duration and security password through a 4×4 matrix keypad, and start the charging process. The compartment remains locked during charging and can only be accessed after successful authentication.

## 🎯 Objectives

- To develop a secure wireless charging facility for smartphones.
- To implement password-based authentication for device protection.
- To control charging duration using a programmable countdown timer.
- To detect smartphone placement and removal using a piezoelectric sensor and SOUND interface.
- To automate compartment locking and unlocking using a servo motor.
- To reduce unauthorized access to smartphones in public charging environments.

## ⚙️ Hardware Components

| S.No | Component | Purpose |
|---|---|---|
| 1 | ESP8266 NodeMCU | Main microcontroller |
| 2 | Mini Servo SG90 | Compartment locking and unlocking |
| 3 | 5V Relay Module | Controls wireless charging power |
| 4 | 4×4 Matrix Keypad | Password and charging-time input |
| 5 | 16×2 LCD with I2C | Displays instructions and status |
| 6 | Piezoelectric Sensor with SOUND Interface | Detects smartphone placement and removal |
| 7 | Wireless Charging Module | Provides wireless power transfer |
| 8 | Buzzer | Provides security alerts |
| 9 | 9V / 2A DC Adapter | Power supply |
| 10 | Breadboard and Connecting Wires | Circuit connections |

## 💻 Software and Technologies Used

- **Arduino IDE:** Used for writing, compiling, and uploading the embedded program.
- **Embedded C/C++:** Used to develop the microcontroller firmware.
- **Wokwi Simulator:** Used to simulate supported circuit components and verify control logic.
- **ESP8266 Board Package:** Enables programming of the NodeMCU board.

## 🔄 Working Principle

The system operates through the following sequence:

1. **System Initialization:** The ESP8266 initializes the keypad, LCD, sensor interface, servo motor, relay, and buzzer.
2. **Phone Detection:** The piezoelectric sensor detects changes in applied pressure when a smartphone is placed on the charging platform.
3. **User Input:** The user enters the required charging duration and security password using the 4×4 keypad.
4. **Authentication:** The controller processes the entered information and verifies the required conditions.
5. **Automatic Locking:** The SG90 servo motor locks the charging compartment.
6. **Wireless Charging:** The relay activates the wireless charging module.
7. **Timer Control:** The LCD displays the charging status and remaining time.
8. **Charging Termination:** When the selected duration expires, the relay automatically switches OFF.
9. **Password Verification:** The user enters the previously configured password to unlock the compartment.
10. **Security Alert:** If an incorrect password is entered, the buzzer generates an alert and the compartment remains locked.
11. **Phone Removal:** The sensor detects the removal of the smartphone, and the system returns to standby mode.

## ⭐ Key Features

- Wireless smartphone charging.
- Password-protected charging compartment.
- Automatic locking and unlocking mechanism.
- User-selectable charging duration.
- Automatic charging termination.
- Smartphone placement detection.
- LCD-based status monitoring.
- Buzzer-based security alerts.
- ESP8266-based embedded control.
- Expandable IoT functionality through Wi-Fi.

## 🏗️ System Architecture

**Input Section:**
- 4×4 Matrix Keypad
- Piezoelectric Sensor with SOUND Interface

**Processing Section:**
- ESP8266 NodeMCU

**Output Section:**
- 16×2 LCD Display
- SG90 Servo Motor
- Relay Module
- Wireless Charging Module
- Buzzer

## 🧪 Simulation and Testing

The Wokwi online simulator is used to verify the supported components and programmed control operations.

The simulation focuses on:

- Keypad input processing.
- LCD message display.
- Servo motor control.
- Relay switching.
- Countdown timer operation.
- Password authentication logic.

The physical prototype is used to evaluate the actual sensor response, wireless charging operation, and electromechanical performance.

**Note:** Piezoelectric sensor operation and wireless power transfer require physical hardware testing or suitable simulation models.

## 💡 Advantages

- Improves smartphone security in public charging areas.
- Eliminates the need for direct charging cable connections.
- Provides controlled charging duration.
- Prevents unauthorized compartment access.
- Offers a simple keypad-based user interface.
- Uses affordable and commonly available components.
- Supports future IoT-based improvements.

## 🌍 Sustainable Development Goals (SDGs)

This project supports the following United Nations Sustainable Development Goals:

- **SDG 9 – Industry, Innovation and Infrastructure:** Promotes embedded-system innovation through integrated wireless charging and security.
- **SDG 11 – Sustainable Cities and Communities:** Supports safer and more convenient shared charging facilities in public places.
- **SDG 12 – Responsible Consumption and Production:** Uses timer-based power control to avoid unnecessary operation of the charging module.

## 🚀 Future Scope

- IoT-based charging-session monitoring.
- Mobile application integration.
- RFID or biometric authentication.
- Multiple charging compartments.
- Improved sensor calibration and detection accuracy.
- Advanced wireless charging safety mechanisms.
- Energy consumption monitoring.
- Remote monitoring through cloud platforms.

## 💰 Estimated Project Cost

| Component | Cost (INR) |
|---|---:|
| ESP8266 NodeMCU | ₹550 |
| 16×2 LCD + I2C Module | ₹250 |
| 4×4 Matrix Keypad | ₹100 |
| SG90 Servo Motor | ₹120 |
| 5V Relay Module | ₹80 |
| Wireless Charging Pad + Coil | ₹350 |
| Buzzer, LED and Resistors | ₹30 |
| Enclosure / Bay Door | ₹400 |
| Adapter, Wires and PCB | ₹250 |
| **Total** | **₹2,130** |

## 👨‍💻 Project Team

**Department:** Electronics and Communication Engineering  
**Institution:** K. Ramakrishnan College of Engineering (Autonomous)  
**Course:** ECB1303 – Embedded Systems & IoT Design

| Name | Register Number |
|---|---|
| Niranjan S | 8115U24EC067 |
| Pranav M | 8115U24EC075 |
| Sasi Dharan M | 8115U24EC100 |
| Vishnu Prasath S | 8115U24EC121 |

**Project Guide:**  
Dr. R. Samson Daniel, M.E., Ph.D.  
Associate Professor, Department of ECE.

## 📌 Conclusion

The Adaptive Time-Locked Wireless Charging Station combines wireless charging, smartphone detection, password authentication, timer-based control, and an automatic locking mechanism into a single embedded system.

By integrating the ESP8266 NodeMCU with sensing and control components, the project provides a practical approach to improving smartphone charging security in public environments.

The project demonstrates how embedded systems and IoT technologies can be used to develop affordable, automated, and secure charging solutions.

---

**Developed as part of ECB1303 – Embedded Systems & IoT Design.**
