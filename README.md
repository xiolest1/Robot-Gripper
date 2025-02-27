# Robot-Gripper

This system enables users to control a **servo motor** using a **GUI (Python Tkinter)** that communicates with an **Arduino microcontroller** via serial communication to control a **3D-printed robotic gripper**. The GUI Allows the user to adjust the servo angle using a slider and sends the commands to the Arduino in real-time.

## **Table of Contents**
- [Features](#features)
- [Installation](#installation)
- [Software Requirements](#software-requirements)
- [Usage](#usage)
  - [Running the Python GUI](#running-the-python-gui)
  - [Uploading the Arduino Code](#uploading-the-arduino-code)
- [How It Works](#how-it-works)


## **Features**
✅ **Graphical User Interface (GUI):** Built with `customtkinter` for an enhanced user experience.  
✅ **Real-Time Servo Control:** Adjust the servo angle dynamically using a slider.  
✅ **Serial Communication:** Uses `pyserial` to send data from Python to the Arduino.  

## Installation

Follow these steps to set up the project:

#### 1. Install Python Dependencies

Ensure you have Python installed, then install the required libraries:

~~~bash
pip install customtkinter pyserial
~~~

#### 2. Connect Arduino

- **Plug your Arduino** into the computer via USB.
- **Identify the COM Port** assigned to it (e.g., `COM10` on Windows or `/dev/ttyUSB0` on Linux/Mac).
- **Update the Python Script:**  
  Open `python_arduino_ctrl_servo.py` and update the port configuration to match the correct COM port.

---

## Software Requirements

- **Python 3.x**  
- **Arduino IDE**  
- **Required Python Libraries:**  
  - `customtkinter`  
  - `pyserial`  

## Usage

### Running the Python GUI

1. **Open a Terminal** in the project folder.  
2. **Run the Python Script:**

   ~~~bash
   python python_arduino_ctrl_servo.py
   ~~~

3. **Interact with the GUI**  
   - Use the slider to set the servo angle (0° - 180°).  
   - Click the **Send Angle** button to move the servo.

### Uploading the Arduino Code

1. **Open the Arduino IDE** and load `arduino_code.ino`.  
2. **Select the Correct Board** (e.g., Arduino Uno, Mega, etc.).  
3. **Select the Correct Port**.  
4. **Click Upload** to flash the code onto the Arduino.

## Pictures + Video testing out the RC Car
<img src="https://i.postimg.cc/bv27ZfkG/robot-Gripper-image1.jpg" width="300" alt="Process Flow">
<img src="https://i.postimg.cc/zBZ9W2Fx/Robot-Gripper-img2.jpg" width="300" alt="Process Flow">
<img src="https://i.postimg.cc/50BDm5Pb/Robot-Gripper-img3.jpg" width="300" alt="Process Flow">

![Screenshot 2025-02-24 070546](https://github.com/user-attachments/assets/3357354d-a819-4adf-a059-d47e851f98bc)

https://github.com/user-attachments/assets/4c52b7bf-6a20-461e-b966-f172d3e883aa

*Click thumbnail to watch demo video ↗️*
[![Watch the Gripper in Action](https://img.youtube.com/vi/uto3_GqsF7M/0.jpg)](https://www.youtube.com/shorts/uto3_GqsF7M)

