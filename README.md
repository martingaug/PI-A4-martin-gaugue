# PI-A4-martin-gaugue
DIGITLED

## Project Description
This project explores a novel way of interacting with sound by using light as a control interface.
A synthesizer is controlled through RGB LEDs and photodiodes: variations in light intensity are captured and converted into electrical signals, which then influence sound generation.

The system creates an expressive and intuitive musical instrument where light becomes a medium for sound design.
The output signal is processed through an analog delay circuit (PT2399), allowing dynamic sound textures and spatial effects.

## Concept

The goal of this project is to design an interactive audio system where:

* Light intensity and color controls sound parameters
* Physical interaction replaces traditional interfaces (knobs, keys)
* The system can be used in artistic installations or live performances

---

## System Overview

1. RGB LEDs emit light
2. Photodiodes receive the light and convert it into electrical signals
3. A comparator (threshold detection) transforms the signal into usable control data
4. The synthesizer generates sound based on these signals
5. The output is processed through a PT2399 delay module
6. The delay parameters can be influenced dynamically

---

## Electronics

### Bill of Materials (BOM)

* Microcontroller (XIAO ESP32S3 / Arduino)
* RGB LEDs
* Photodiodes (e.g., BPW21R)
* Resistors
* Potentiometer (optional)
* Comparator (LM311)
* Operational amplifier (LM358 / TL062)
* PT2399 Delay IC
* Capacitors
* Audio output (jack / speaker)
* Breadboard and wires

---

##  Assembly Instructions

1. Connect RGB LEDs to the microcontroller (PWM pins)
2. Place photodiodes facing the LEDs
3. Connect photodiodes to a comparator (LM311) with a defined threshold (~400mV)
4. Feed the comparator output into the synthesizer control input
5. Build or connect the synthesizer circuit
6. Add the PT2399 delay circuit at the output
7. Connect to an audio output (speaker or audio interface)

---

## Software / Firmware

The microcontroller controls:

* LED colors and intensity
* Interaction mapping (light → sound)

### How to run

1. Open the `.ino` file in Arduino IDE
2. Select the correct board (ESP32 / Arduino)
3. Upload the code
4. Power the system

---

## How It Works

The system is based on light-to-voltage conversion:

* Photodiodes generate a current proportional to light intensity
* The comparator detects when a threshold is reached
* This signal triggers or modulates the synthesizer
* The delay (PT2399) adds temporal and spatial effects

---

## 👤 Author

Martin – ESILV Engineering Student (Createch)
Music Producer & Creative Technologist

---
