# smart-pet-feeder-system
A bare-metal ATmega16 automatic pet feeder project with loadcell, RTC, servo.
# Smart Pet Feeder System 

An automatic pet feeder project I built as part of my embedded systems coursework. The system uses a load cell to measure food weight and an RTC for scheduling, all controlled by an ATmega16A.

---

##  System Architecture & Hardware Specifications

The system is designed around a central microcontroller that handles real-time clock inputs, structural weight sensor filtering, and PWM actuation:

* **Microcontroller:** .ATmega16A (Bare-metal C)
* **Peripherals:** RTC DS1307 (I2C), HX711 ADC (Load cell), SG90 Servo (PWM)
* **User Interface:** 16x2 LCD, 4x4 Keypad
* **PCB Design:** Altium Designer (Single-layer)

---

##  System Design Details

### Hardware Block Diagram
Below is the structural layout illustrating how the peripheral units interact with the main MCU core:

![System Block Diagram](images/block_diagram.png)

---

##  Project Gallery & Results

### Circuit Simulation & PCB Design
The system was successfully simulated and modeled before physical fabrication. The PCB layout consists of a optimized single-layer routing designed for seamless manual etching.

| Proteus Simulation | Altium PCB Layout | 3D Board Visualization |
| :---: | :---: | :---: |
| ![Proteus Simulation](images/proteus_simulation.png) | ![PCB Layout](images/pcb_layout.png) | ![3D View](images/pcb_3d.png) |

### Physical Prototype
The final system achieved a top 3 ranking in excellence during class presentation, demonstrating highly stable operational feedback.

| Breadboard Testing | Final PCB Assembly | Mechanical Enclosure Model |
| :---: | :---: | :---: |
| ![Breadboard Test](images/breadboard.png) | ![Assembled PCB](images/final_pcb.png) | ![Enclosure Model](images/enclosure.png) |

---

##  Future Enhancements
* **IoT Upgrade:** Integrating an ESP32/ESP8266 Wi-Fi module for cloud synchronization and remote app-based configurations.
* **Closed-Loop Bowl Monitor:** Installing an infrared or proximity sensor on the feeding tray to prevent over-dispensing when food is left over.
* **Power Redundancy:** Introducing a secondary battery backup line to secure feeding operations during standard blackouts.


##  My Contributions
As a core member of the team, I wore several hats to bridge the gap between our **hardware**, **firmware**, and **mechanical design**. My primary focus was ensuring that the different layers of the project actually played nice with each other.

I handled the low-level C development for the servo motors and buzzer alerts, while also getting hands-on with the PCB assembly—soldering everything myself to ensure the connections were solid. Beyond the electronics, I built out the housing and integrated the control board with the mechanical dispensing gate. A big part of my role was also the 'messy' side of the project: troubleshooting hardware glitches and debugging firmware quirks to get the system stable. Finally, I mapped out our software architecture through flowcharts and pulled together our final engineering report to document how all the pieces fit together.
