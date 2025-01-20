---
title: "Automated Syringe Pump"
excerpt: "A linear actuator-controlled syringe pump"
header:
  image: assets/img/Syringe Pump Final.jpg
  teaser: assets/img/Syringe Pump Final.jpg
gallery:
  - image_path: assets/img/Syringe Pump Render.png
  - image_path: assets/img/Syringe Pump Final.jpg
  - image_path: assets/img/Syringe Pump Circuit Schematic.png
   
---

## Overview

The Syringe Pump Project was developed as part of the DF 2100: Rapid Prototyping course in Fall 2023. My team, the ABS Absurdists, designed and constructed a laboratory-grade syringe pump capable of dispensing fluid at a calculated and constant flow rate.

This automated linear actuator-controlled syringe pump offers precise and accurate flow rates over extended periods, minimizing cross-contamination and allowing for the administration of viscous liquids. The pump is primarily designed for use in medical, biomedical, and chemical contexts, where exact fluid dispensation is crucial.

## Gallery

{% include gallery caption="Original 3D render, final product, and circuit schematic." %}

## Features

- Accommodates syringes between 5-20 mL
- Easy syringe interchangeability
- Stepper motor-driven lead screw mechanism
- Arduino-controlled operation
- LED status indicator (Green: Running, Yellow: Paused, Red: Empty)
- User-friendly controls:
  - Two latching push buttons (Power and Pause)
  - Two momentary buttons (Direction control)
  - Rotary potentiometer (Flow rate control)
- Limit switch for automatic stop at syringe empty state
- Water-resistant enclosure for electronics
- Custom 3D printed components
- Minimum flow rate of 7.06E-5 ml/min (with 5 mL syringe)
- Flow rates up to 10.63 mL/min (with 20 mL syringe)

## 3D Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a409283e542283b188?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Purchased Components

| Component | Quantity | Purpose |
|-----------|----------|---------|
| Arduino UNO | 1 | Main controller |
| Small Breadboard | 1 | Electronics |
| A4988 Stepper Driver | 1 | Electronics |
| Nema 17 Stepper Motor | 1 | Drive mechanism |
| 250 mm Lead Screw with 2 mm pitch and 8 mm lead | 1 | Linear motion |
| 1/4" x 8mm Flexible Coupling | 1 | Rotary shaft connection |
| 200 mm Linear Rod with 8mm diameter | 1 | Guidance and stability |
| Flexible Coupler | 1 | Motor to lead screw connection |
| Lead Screw Nut | 1 | Carriage movement |
| Flange Bearings | 2 | Lead screw support |
| LM8UU Linear Bearing for 8 mm Diameter Rod| 2 | Carriage movement |
| MEAN WEL RQ-65D Power Supply | 1 | Power source |
| Common Cathode LED | 1 | Status indicator |
| Latching Push Buttons | 2 | Power and pause control |
| Momentary Push Buttons | 2 | Direction control |
| Rotary Potentiometer | 1 | Flow rate control |
| Limit Switch | 1 | End-of-travel detection |
| Aluminum Extrusion | 1 | Structural support & mount |
| M5 Machine Screws | 12 | Case assembly |
| M5 Heat Set Inserts | 12 | Case assembly |
| O-Ring for M5 Screw | 4 | Waterproofing enclosure top |

## Custom 3D Printed Components

| Component | Material | Purpose |
|-----------|----------|---------|
| Motor Mount | ABS | Houses motor, couplings, and bearings |
| Carriage | ABS | Holds syringe plunger and moves along lead screw |
| End Support | ABS | Supports syringe body and bearings |
| Barrel Support | ABS | Holds syringe barrel |
| Lead Screw Cover | ABS | Aesthetic cover for unused lead screw portion |
| Enclosure Base | PLA | Houses electronics |
| Front Panel | PLA | Holds user interface components |
| Enclosure Top | PLA | Secures aluminum extrusion |
| Back Panel | PLA | Completes the protective casing |

## Arduino Code

The Arduino code controls the syringe pump's operation, including motor speed, direction, and LED status indicators. It uses the AccelStepper library for precise stepper motor control and includes functions for calculating flow rates based on syringe size and motor speed.

Key features of the code include:
- Configurable syringe diameter and lead screw parameters
- Real-time flow rate calculation and serial output
- Button and potentiometer input handling
- LED color control for status indication
- Limit switch integration for safety

You can find the full Arduino code in our [GitHub repository](https://github.com/TommyPennington/syringepump)

## Operating Instructions

1. Connect the power supply to a standard 120 V wall socket.
2. Connect the Arduino UNO to a computer via USB cable.
3. Upload the Arduino code, ensuring the correct syringe diameter is set in the `SYRINGE_DIAMETER` variable.
4. Load the desired syringe (5-20 mL) into the pump.
5. Press the power button (rightmost) to initialize the program.
6. Use the pause button (second from right) to start/stop the pump.
7. Adjust the flow rate using the potentiometer dial.
8. Use the two leftmost momentary buttons to manually control the direction when the pump is stopped.
9. The LED indicator will show the pump status:
   - Green: Running
   - Yellow: Paused
   - Red: Syringe empty or limit switch activated

Note: When the syringe is empty, the pump will automatically stop. Use the direction control buttons to reset the pump position before loading a new syringe.
