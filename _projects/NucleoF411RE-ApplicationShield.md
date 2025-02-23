---
layout: page
title: NucleoF411RE-ApplicationShield
description: 🎛️ Nucleo F411RE synth project!
full_name: mpek29/NucleoF411RE-ApplicationShield
img: assets/img/projects/NucleoF411RE-ApplicationShield/main.png
importance: 1
git: https://github.com/mpek29/NucleoF411RE-ApplicationShield
category: Computer Science
subcategory: Firmware Development
---


**NucleoF411RE-ApplicationShield** is an open-source firmware project designed to leverage the **Nucleo-F411RE** development board in conjunction with the **Application Shield** from ARMmbed. This project aims to assemble a comprehensive codebase that explores all the functionalities offered by the combination of the Nucleo-F411RE and the Application Shield.

## 🎯 Purpose

- 🔌 **GPIO Control**: Interact with GPIO pins for reading, writing values, and generating PWM signals.
- ⏱️ **Timer Management**: Utilize timers to detect short and long button presses.
- ⚡ **Interrupt Handling**: Implement timer and button press interrupts for dynamic LED control.
- 💬 **Serial Communication**: Facilitate communication between the computer and the Nucleo board.
- 🌡️ **Sensor Interaction**: Communicate via I2C and SPI to gather data from sensors and control displays.
- 🔄 **ADC Utilization**: Read analog values from potentiometers.

## 📝 Features

| 🏷️ Feature                | 🔍 Description                                 |
|--------------------------|-----------------------------------------------|
| 💡 **GPIO Control**       | Read/write values and generate PWM signals.   |
| ⏲️ **Timer Management**    | Manage timers TIM2 to TIM5 for button presses. |
| ⚠️ **Interrupts**         | Use interrupts for LED blinking and button actions. |
| 💻 **Serial Communication** | Communicate with the Nucleo board via serial. |
| 🌡️ **I2C Communication**  | Retrieve temperature from the LM75 sensor and interact with MMA7660 accelerometer. |
| 📺 **SPI Communication**   | Control an LCD display using SPI.             |
| 🎚️ **ADC Usage**         | Read potentiometer angles through ADC.        |

## 🎛️ Example Applications

1. **GPIO Test**: Read/write values and generate PWM to control LED brightness on the board.
2. **Button Press Detection**: Utilize timers to differentiate between short and long presses on a push button.
3. **LED Blinking with Interrupts**: Implement interrupt-driven blinking of an LED based on timer events or button presses.
4. **Serial Communication**: Establish communication between the computer and Nucleo-F411RE for data exchange.
5. **I2C Temperature Reading**: Communicate with the LM75 temperature sensor and MMA7660 accelerometer via I2C.
6. **SPI LCD Control**: Use SPI to manage an LCD display connected to the development board.
7. **ADC Potentiometer Reading**: Capture the angle of potentiometers using the ADC.

## 📐 System Architecture

| 🔌 GPIO Control | ⏲️ Timer Management | ⚠️ Interrupts | 💬 Serial Communication |
|----------------|---------------------|---------------|------------------------|
| Control LEDs and buttons | Manage button press timing | Trigger actions on interrupts | Exchange data with the computer |

## 📜 Code Structure

```bash
📁 NucleoF411RE-ApplicationShield/
├── 📂 Core/
│   ├── main.c        # Main firmware loop
│   ├── gpio.c        # GPIO handling and PWM
│   ├── timers.c      # Timer management
│   ├── interrupts.c   # Interrupt handling
│   ├── serial.c      # Serial communication control
│   ├── i2c.c         # I2C communication
│   ├── spi.c         # SPI communication for LCD
│   ├── adc.c         # ADC handling
├── 📂 Drivers/        # Nucleo HAL libraries
├── 📂 Inc/           # Header files
├── 📂 Assets/        # UI elements, example configurations
└── README.md         # This file
```

