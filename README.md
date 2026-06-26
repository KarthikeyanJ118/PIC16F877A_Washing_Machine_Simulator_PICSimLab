# 🧺 Washing Machine Simulator using PIC16F877A

> A microcontroller-based washing machine simulation developed using the **PIC16F877A**. The project demonstrates the implementation of an **Embedded Finite State Machine (FSM)** to control washing operations such as program selection, water level management, washing, rinsing, spinning, and cycle completion.

---

## 📖 Project Overview

This project simulates the working of an automatic washing machine using the **PIC16F877A** microcontroller. The system provides multiple wash programs, configurable water levels, and timer-based cycle management. A **16×2 Character LCD (CLCD)** displays the current operating state, while tactile switches allow users to interact with the system.

The firmware is developed in **Embedded C** using **MPLAB X IDE** and **XC8 Compiler**, and tested using **PICSimLab**.

---

## ✨ Features

* 🧺 Multiple washing programs (Daily, Heavy, Delicates, Whites)
* 💧 Adjustable water level selection
* ⏱️ Timer-based wash cycle management
* 📺 16×2 CLCD for real-time status display
* 🔘 Push-button user interface
* 🚪 Door safety simulation
* ⏸️ Start, Pause and Resume functionality
* 🔔 Buzzer notification on cycle completion
* ⚙️ Finite State Machine (FSM) based control logic

---

## 🛠 Hardware Requirements

| Component           | Description             |
| ------------------- | ----------------------- |
| 🧠 PIC16F877A       | Microcontroller         |
| 📺 16×2 CLCD        | Display Module          |
| 🔘 Tactile Switches | User Inputs             |
| ⚙️ DC Motor         | Washing Drum Simulation |
| 🔔 Buzzer           | Audio Notification      |
| 🔋 Power Supply     | 5V                      |
| 🔌 Connecting Wires | Circuit Connections     |

---

## 💻 Software Requirements

* 🖥️ MPLAB X IDE
* ⚙️ XC8 Compiler
* 🔬 PICSimLab
* 💻 Embedded C

---

## ⚙️ System Workflow

### 🔹 Power ON

* Display welcome message
* Initialize peripherals

### 🔹 Program Selection

* Choose washing mode
* Select water level

### 🔹 Washing Cycle

* Start motor
* Display remaining time
* Monitor system status

### 🔹 Pause Mode

* Pause timer
* Stop motor safely

### 🔹 Completion

* Stop motor
* Activate buzzer
* Display **Program Complete**
* Return to Home Screen

---

## 🔄 Finite State Machine (FSM)

```text
Power ON
     │
     ▼
Program Selection
     │
     ▼
Water Level Selection
     │
     ▼
Start Program
     │
     ▼
Wash
     │
     ▼
Rinse
     │
     ▼
Spin
     │
     ▼
Program Complete
     │
     ▼
Return to Home
```

---

## 📂 Project Structure

```text
Washing-Machine-Simulator/
│
├── 📄 README.md
├── 📂 Source_Code/
│   ├── main.c
│   ├── lcd.c
│   ├── keypad.c
│   ├── timer.c
│   ├── interrupt.c
│   ├── washing_machine.c
│   └── config_bits.c
│
├── 📂 Header_Files/
│   ├── lcd.h
│   ├── keypad.h
│   ├── timer.h
│   ├── interrupt.h
│   └── washing_machine.h
│
├── 📂 Simulation/
│   ├── WashingMachine.hex
│   └── WashingMachine.pzw
│
├── 📂 Images/
│   ├── powering_on_screen.png
│   ├── washing_programs_screen.png
│   ├── water_level_screen.png
│   ├── program_running.png
│   ├── pause_screen.png
│   └── program_complete.png
│
└── 📜 LICENSE
```

---

## 🚀 Setup & Installation

### 1️⃣ Build the Project

* Open the project in **MPLAB X IDE**
* Select **PIC16F877A**
* Build the project using **XC8 Compiler**
* Generate the `.hex` file

### 2️⃣ Run Simulation

* Open **PICSimLab**
* Select **PICGenios** board
* Choose **PIC16F877A**
* Load the generated `.hex` file

### 3️⃣ Test the System

* Select a washing program
* Choose water level
* Start the cycle
* Observe LCD status and timer
* Pause/Resume using switches
* Wait for completion notification

---

## 🖼 Simulation Screens

### 🔋 Power ON

<img src="images/powering_on_screen.png" width="350">

### 🧺 Program Selection

<img src="images/washing_programs_screen_1.png" width="350">

### 💧 Water Level Selection

<img src="images/water_level_screen_1.png" width="350">

### ⏱ Running Program

<img src="images/program_and_time_display.png" width="350">

### ⏸ Pause State

<img src="images/program_paused_screen.png" width="350">

### ✅ Program Complete

<img src="images/program_complete_screen.png" width="350">

---

## 📚 Learning Outcomes

* Embedded C Programming
* PIC16F877A Programming
* MPLAB X IDE
* XC8 Compiler
* Finite State Machine (FSM)
* Timer Programming
* Interrupt Handling
* LCD Interfacing
* Switch Debouncing
* Embedded System Design
* Hardware Simulation using PICSimLab

---

## 🎯 Applications

* 🧺 Home Appliance Automation
* 🏭 Embedded Control Systems
* 🎓 Academic Mini Projects
* 💼 Embedded Firmware Learning
* 🧪 Industrial Process Simulation

---

## 🔮 Future Enhancements

* 🌡 Temperature Sensor Integration
* 📶 IoT Monitoring using ESP32
* 📱 Mobile Application Control
* ☁ Cloud Data Logging
* 💦 Automatic Water Level Detection
* ⚡ Energy Consumption Monitoring

---

## 👨‍💻 Author

**Karthikeyan J**

🎓 B.E. Electronics and Communication Engineering

💼 Embedded Systems | Embedded C | Firmware Development | PIC Microcontrollers | IoT

---

## 📄 License

This project is developed for **educational and learning purposes**.

⭐ If you found this project useful, consider giving it a **Star** on GitHub!
