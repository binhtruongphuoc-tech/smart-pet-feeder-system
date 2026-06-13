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
##  My Contributions
I worked across the **hardware**, **firmware**, and **mechanical sides** to get everything synced up. I wrote the C drivers for the servo and buzzer, and hand-soldered the PCB myself for a clean, reliable build. I also handled the housing and integration with the dispensing gate. A big part of the job was just grinding through the 'messy' stuff—debugging hardware glitches and firmware quirks to get the system stable. I wrapped it all up by documenting the architecture and writing the final report.
