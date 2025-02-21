---
layout: page
title: MicroUSB2DIP
description: 🔌 Micro USB to DIP reverse-engineered
img: assets/img/projects/MicroUSB2DIP/main.png
importance: 1
git: https://github.com/mpek29/MicroUSB2DIP
category: Electronics
subcategory: PCB Reverse Engineering
---



# MicroUSB2DIP

## 🚀 Overview
![Main Preview](assets/img/main.png)

This is an open-source reverse-engineered version of a Micro USB to DIP adapter, based on the original component available [here](https://fr.aliexpress.com/item/32947889760.html). The goal of this project was to practice reverse engineering as a learning exercise and to prepare for a future adaptation in a larger project.

## 🎯 Purpose
- 🔍 **Reverse engineering**: Understanding the design and functionality of this micro USB  to DIP connector.
- 🛠️ **Skill development**: Enhancing expertise in PCB design and hardware analysis skills.
- 🔄 **Future adaptation**: Leveraging this knowledge for embedded applications.

## 📝 Features Comparison: Original vs. Reverse-Engineered

| Feature            | Original Module | Reverse-Engineered Version |
|--------------------|----------------|---------------------------|
| 🖥️ PCB Design        | Proprietary     | Open-source & customizable |
| 🔌 Connector Type    | Micro USB       | Micro USB |
| 📌 Pin Mapping      | Standard DIP    | Standard DIP |
| 👐 Mechanical Drawing  | {% include image.html path="assets/img/projects/MicroUSB2DIP/original_pcb.png" width="300" height="300" %} | {% include image.html path="assets/img/projects/MicroUSB2DIP/reversed_pcb.png" width="300" height="300" %} |
| 📝 Reverse-Engineered Schematic | N/A | {% include image.html path="assets/img/projects/MicroUSB2DIP/reversed_sch.png" width="300" height="300" %} |
| 📷 Photo             | {% include image.html path="assets/img/projects/MicroUSB2DIP/original_3d.png" width="300" height="300" %} | {% include image.html path="assets/img/projects/MicroUSB2DIP/reversed_3d.png" width="300" height="300" %} |

## 🛠️ How to Use
### 📌 Wiring Guide

| Pin  | Function |  
|------|----------|  
| VBUS | +5V |  
| D-   | Data - |  
| D+   | Data + |  
| ID   | Mode detect (A: GND, B: Open) |  
| GND  | Ground |  

## 🌟 License
This project is open-source. Feel free to use, modify, and contribute! 🚀

