# Washing Machine Simulator using PIC16F877A

## ➢ Project Overview
This project is a functional simulation of a washing machine control system. Developed using the **PIC16F877A** microcontroller, it simulates various wash cycles, water level management, and timing controls. The system utilizes a **Finite State Machine (FSM)** approach to manage different states like Power On, Function Selection, and Operation.

## ➢ Key Features
* **Multiple Wash Programs:** Pre-set modes for Daily, Heavy, Delicates, and Whites.
* **User Interface:** Integrated **16x2 CLCD** for real-time status updates and cycle countdowns.
* **Control Inputs:** Tactile switches for program selection, start/pause, and water level settings.
* **Automated Cycle Management:** * **Wash/Rinse/Spin:** Sequenced stages with dedicated timers.
    * **Door Sensing:** Safety simulation that pauses the operation if the door is "opened."
* **Buzzer Alerts:** Audio notifications for cycle completion and error states.

## ➢ Technical Stack
* **Microcontroller:** PIC16F877A
* **Development Tools:** MPLAB X IDE, XC8 Compiler
* **Simulation Environment:** PICSimLab
* **Peripherals used:** Timers (Timer2 for PWM/Clock), External Interrupts, 16x2 CLCD, Tactile Switches, DC Motor (to simulate the drum).
* **Language:** Embedded C

## ➢ System Logic (State Machine)
1.  **Power On State:** Displays a welcome message and waits for user input.
2.  **Selection State:** User chooses the wash program and water level.
3.  **Running State:** Activates the motor and starts the countdown timer based on the selected program.
4.  **Pause State:** Temporarily stops the timer and motor via external interrupts.
5.  **Completion State:** Triggers the buzzer and resets the system to the initial state.

## ➢ Setup & Installation
1.  **Compile:** Build the project in **MPLAB X IDE** to generate the `main.hex` file.
2.  **Simulate:** * Open **PICSimLab** and select the **PICGenius** board.
    * Set the processor to **PIC16F877A**.
    * Load the `.hex` file.
3.  **Interact:** Use the digital switches to select modes and the onboard LCD to monitor the progress.

## ➢ Visual Walkthrough (Simulation Screens)

<table>
  <tr>
    <td><b>1. Powering On</b><br><img src="https://github.com/Pranowmya/Washing-Machine-Simulation-/blob/main/powering_on_screen.png?raw=true" width="250"></td>
    <td><b>2. Program Selection</b><br><img src="https://github.com/Pranowmya/Washing-Machine-Simulation-/blob/main/washing_programs_screen_1.png?raw=true" width="250"></td>
    <td><b>3. Water Level Setup</b><br><img src="https://github.com/Pranowmya/Washing-Machine-Simulation-/blob/main/water_level_screen_1.png?raw=true" width="250"></td>
  </tr>
  <tr>
    <td><b>4. Cycle Running</b><br><img src="https://github.com/Pranowmya/Washing-Machine-Simulation-/blob/main/program_and_time_display.png?raw=true" width="250"></td>
    <td><b>5. Start/Stop Control</b><br><img src="https://github.com/Pranowmya/Washing-Machine-Simulation-/blob/main/start_stop_screen.png?raw=true" width="250"></td>
    <td><b>6. Paused State</b><br><img src="https://github.com/Pranowmya/Washing-Machine-Simulation-/blob/main/program_paused_screen.png?raw=true" width="250"></td>
  </tr>
</table>
<p align="center"><b>7. Program Complete</b><br><img src="https://github.com/Pranowmya/Washing-Machine-Simulation-/blob/main/program_complete_screen.png?raw=true" width="400"></p>