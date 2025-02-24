---
layout: page
title: HeaterControl-Shield
description: 🔥 STM32 Shield for Heat Control
full_name: mpek29/HeaterControl-Shield
img: assets/img/projects/HeaterControl-Shield/main.png
importance: 1
git: https://github.com/mpek29/HeaterControl-Shield
category: Electronics
subcategory: PCB Design
---


**HeaterControl-Shield** is an open-source electronic board designed to control a **heating resistor**, measure the **consumed current**, and detect the **temperature** near the heating resistor. This board is shaped as an **Arduino shield** and optimized for use with an **STM32 Nucleo**.

## 🎯 Main Features

- 🔥 **Heating resistor control** via an **N-channel MOSFET**.
- ⚡ **Current consumption measurement** using a **shunt resistor** and an **operational amplifier**.
- 🌡️ **Temperature sensing** using a **thermistor** integrated into a **Wheatstone bridge**, amplified by an **instrumentation amplifier**.
- 🛠️ **Open-source and customizable design** to adapt to specific project needs.

## 📝 Technical Specifications

| 🏷️ Feature | 🔍 Description |
|----------------|-------------|
| 🔌 **Power Input** | 5V - 12V |
| 🔥 **Heating Control** | N-channel MOSFET for power control |
| ⚡ **Current Measurement** | Shunt resistor + Operational amplifier |
| 🌡️ **Temperature Sensing** | Wheatstone bridge + Instrumentation amplifier |
| 🔄 **Interface** | Compatible with **Arduino Shield** and **STM32 Nucleo** |
| 🖥️ **PCB Design** | Open-source & customizable |
| 🌍 **Applications** | Thermal control projects, embedded systems, temperature regulation |

## 📐 PCB Preview

| 📜 Schematic | 🖥️ PCB Layout | 🏗️ 3D View |
|-----------|-----------|-----------|
| {% include image.html path="assets/img/projects/HeaterControl-Shield/schematic.png" width="300" %} | {% include image.html path="assets/img/projects/HeaterControl-Shield/pcb_layout.png" width="300" %} | {% include image.html path="assets/img/projects/HeaterControl-Shield/3d.png" width="300" %} |

## 🔗 Main Connections

| Pin | Function |
|-----|---------|
| VIN | Main power input |
| GND | Ground |
| HEAT_CTRL | PWM signal to activate heating |
| CURR_SENSE | Amplified output of current measurement |
| TEMP_SENSE | Amplified output of temperature measurement |

