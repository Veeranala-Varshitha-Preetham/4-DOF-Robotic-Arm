#  4 DOF Robotic Arm

##  Project Overview
This project involves the design and implementation of a **4 Degrees of Freedom (DOF) Robotic Arm** controlled using an **Arduino Uno** and **servo motors**. The arm is designed to replicate human arm motion, with precise and programmable movements for tasks such as picking, placing, and rotating objects.

Developed as part of the *Machines and Mechanisms Lab Project*, the robotic arm demonstrates key mechanical, electrical, and programming principles of mechatronic systems.



---

##  Components Used
### 1. **PWM Servo Motor**
- Voltage (VCC): 3.3–5V  
- Voltage (V+): 4.8–6VDC  
- Current: 6mA (400mA with controller)

### 2. **Arduino Uno**
- Microcontroller: ATmega328  
- Operating Voltage: 5V  
- Input Voltage: 7–12V  
- Flash Memory: 32KB  
- Digital I/O Pins: 14 (6 PWM output)  
- Analog Inputs: 6  

### 3. **Power Supply**
- Input: AC 100–264V, 50/60Hz  
- Output: 5V DC, 2A  
- Power: 25W  

### 4. **Servo Motor**
- Weight: 9g  
- Size: 22×11.5×27 mm  
- Operating Speed: 0.12 sec/60° (at 4.8V)  
- Stall Torque: 1.2 kg/cm  

---

##  Working Principle
The robotic arm operates on **Pulse Width Modulation (PWM)** control for its servo motors, with the **Arduino Uno** generating PWM signals to control each joint:

1. **Base Rotation (DOF 1):** Rotates the arm horizontally.  
2. **Shoulder Movement (DOF 2):** Moves the arm up and down.  
3. **Elbow Movement (DOF 3):** Extends or retracts the arm.  
4. **Gripper Rotation/Control (DOF 4):** Opens/closes or rotates the end-effector.

By adjusting the pulse width, each motor achieves a specific angular position, allowing precise movement and coordination of the arm.

---

##  Kinematic Analysis
The **degree of freedom (DOF)** is calculated using:
DOF = 3(n - 1) - 2j - h

For this arm:  
- n = 5 links  
- j = 4 joints  
- h = 0 higher pairs  

**DOF = 4**, confirming a four-degree system allowing multi-axis movement.

---

##  Future Enhancements
- **Bluetooth Control:** Add wireless control for remote operation.  
- **Potentiometer Interface:** Enable manual joint control using variable resistors.  
- **AI Integration:** Implement vision-based feedback for object detection and autonomous tasks.

---

##  Advantages
- Continuous, fatigue-free operation.  
- High accuracy and repeatability.  
- Enhanced safety by automating hazardous tasks.  
- Reconfigurable for different applications.  

---

##  Limitations
- Limited range and reach due to only 4 DOF.  
- Reduced flexibility in complex manipulations.  
- May face difficulties avoiding obstacles.

---

##  Applications
- Assembly line automation  
- Precision pick-and-place tasks  
- Research and education in robotics  
- Medical and surgical assistance  

---

##  Tools and Software
- **Arduino IDE** for programming  
- **C/C++** for microcontroller code  
- **SolidWorks/AutoCAD** for mechanical design (optional)  

---

##  Conclusion
This 4 DOF robotic arm demonstrates how electromechanical systems can replicate human motion through coordinated servo control. By combining mechanical design, embedded systems, and control logic, this project showcases the potential of automation for industrial and research applications.

---



##  Repository Structure

├── README.md
│
├── code/
│   ├── robotic_arm.ino
│
├── circuit/
│   ├── schematic.png
│
└── Documentation/
│   ├── Presentation.ppt
│   ├── Report.pdf


---

##  License
This project is for educational purposes.  
You may modify or use it for learning or non-commercial development with proper credit to the original authors.

---

##  Acknowledgments
We express our gratitude to our mentors and lab coordinators for their guidance and support during this project.

