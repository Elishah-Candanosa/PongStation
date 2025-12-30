# PongStation: Hybrid Arduino-Python Console

* **Author:** Elishah Candanosa
  

**PongStation** is a hardware-software reimplementation of the classic 1972 *Pong* video game, built effectively from scratch to demonstrate the integration of analog electronics, real-time serial communication, and vector physics.

<div align="center">
  <img width="616" height="448" alt="image" src="https://github.com/user-attachments/assets/db1bfff3-eb99-4a2c-a2fc-10a6ec506a7b" />
</div>


## Abstract
This work presents the design, construction, and programming of the "PongStation," a reimplementation of the classic 1972 Pong video game using a hybrid architecture combining an Arduino Uno microcontroller and a Python execution environment. Notably, it offers the flexibility to play on either an **I2C OLED Display** or a **Laptop screen**.

This project centers on a complex system integrating analog and digital electronic components, including sliding potentiometers, an SH1106 I2C OLED display, and a passive buzzer. The console is managed via a serial communication protocol optimized for real-time operation with no perceptible latency, ensuring gameplay is as fluid as attainable with an Arduino UNO.

Unlike traditional implementations, this project introduces a custom physics engine that replaces simple rectangular collisions with **elliptical paddles**, applying vector calculus to determine velocity reflection. The results demonstrate a robust system capable of operating in two game modes—*Monitor* and *OLED*—covering both visualization and sound.

## Key Features
* **Hybrid Architecture:** Arduino handles input/output (ADC/DAC) while Python manages the game logic and physics engine.
* **Dual Display Modes:**
    * **OLED Mode:** Renders graphics on a 1.3" SH1106 display via I2C.
    * **Monitor Mode:** Renders high-resolution graphics on a PC screen using Python (Pygame).
* **Advanced Physics:** Implements elliptical collision detection and vector velocity reflection instead of standard bounding boxes.
* **Low-Latency Serial Protocol:** Custom byte-stream optimization for lag-free control.

## Hardware Components
* **Microcontroller:** Arduino Uno
* **Input:** 2x Sliding Potentiometers (Analog control for paddles)
* **Button:** To start and exit game.
* **Display:** SH1106 I2C OLED Display (128x64)
* **Audio:** Passive Buzzer (PWM sound generation)
* **Wiring:** Breadboard and jumpers for circuit integration

## Installation & Usage

1.  **Hardware Setup:**
2.  **Firmware:**
    * Upload the `pong_firmware.ino` sketch to the Arduino Uno.

3.  **Software:**
    * Run the Python Script on your Laptop. **Be aware that a UNIX environment is expected, if your device has Windows, it might still work changing the port in the Python Script.**


---

If you have any questions, feel free to contact me through my institutional email!

carlos.candanosa@correo.nucleares.unam.mx
