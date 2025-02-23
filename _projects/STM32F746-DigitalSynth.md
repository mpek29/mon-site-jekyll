---
layout: page
title: STM32F746-DigitalSynth
description: 🎹 Digital synth for STM32F746
full_name: mpek29/STM32F746-DigitalSynth
img: assets/img/projects/STM32F746-DigitalSynth/main.png
importance: 1
git: https://github.com/mpek29/STM32F746-DigitalSynth
category: Computer Science
subcategory: Firmware Development
---


**STM32F746-DigitalSynth** is an open-source firmware designed to turn the **STM32F746 Discovery Board** into a powerful subtractive synthesizer. This project generates harmonically rich waveforms and applies **low-pass filtering** to shape the sound dynamically based on the played note.

## 🎯 Purpose

- 🎹 **Digital subtractive synthesis**: Generates a waveform and filters harmonics to create rich sounds.
- 🎛️ **Real-time sound processing**: Implements **FIR and IIR filters** for smooth sound shaping.
- ⚡ **Optimized for STM32F746**: Utilizes the **ARM Cortex-M7 DSP capabilities** for efficient audio processing.
- 🛠️ **Open-source and customizable**: Modify and adapt the code to fit your needs.

## 📝 Features

| 🏷️ Feature        | 🔍 Description |
|----------------|-------------|
| 🎶 **Waveforms** | Triangle, Sawtooth, Square |
| 🎵 **Frequency Control** | MIDI note-based tuning |
| 🎚️ **Low-Pass Filtering** | FIR and IIR-based real-time filtering |
| ⚡ **Processing Unit** | STM32F746 ARM Cortex-M7 |
| 🎛️ **User Interaction** | MIDI input, UI with touchscreen support |
| 🔊 **Audio Output** | 16-bit DAC or I2S codec |
| 🖥️ **DSP Optimization** | ARM CMSIS-DSP library |
| 🌍 **Use Cases** | Digital music synthesis, sound design, embedded audio |

## 🎵 Signal Processing Pipeline

1. **Waveform Generation**: Generates **Triangle, Sawtooth, and Square** waveforms with fundamental frequency based on the input MIDI note.
2. **Low-Pass Filtering**:
   - **FIR Filter**: Provides linear phase response for smooth frequency shaping.
   - **IIR Filter**: Offers efficient real-time filtering with adjustable resonance.
3. **Audio Output**: Sends the processed signal to the **DAC** or external audio codec for playback.

## 📐 System Architecture

| 🎹 MIDI Input | 🎼 Waveform Generation | 🎛️ Filtering | 🔊 Audio Output |
|-----------|-----------|-----------|-----------|
| User plays a note | Generates a rich waveform | Applies FIR & IIR low-pass filtering | Sends audio to DAC or I2S codec |

## 📜 Code Structure

```bash
📁 STM32F746-DigitalSynth/
├── 📂 Core/
│   ├── main.c  # Main firmware loop
│   ├── synth.c  # Waveform generation
│   ├── filter.c  # FIR & IIR filters
│   ├── midi.c  # MIDI note handling
│   ├── dac.c  # Audio output control
├── 📂 Drivers/  # STM32 HAL and CMSIS-DSP libraries
├── 📂 Inc/  # Header files
├── 📂 Assets/  # UI elements, presets
└── README.md  # This file
```

