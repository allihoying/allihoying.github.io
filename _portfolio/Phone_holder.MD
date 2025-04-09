---
title: "Syringe Pump"
excerpt: "Syringe pump capable of delivering flow rates from 1 uL / min to 10 mL / min"
header:
  image: assets/img/Syringe_pump.jpg
  teaser: assets/img/render syringe pump.jpg
gallery:
  - image_path: assets/img/Syringe_pump.jpg
  - image_path: assets/img/render syringe pump.jpg
   
---

## Overview

This syringe pump was created as part of Vanderbilt's rapid prototyping class. The pump is capable of delivering consistant flow rates between 1 uL / min and 10 mL / min for either a large syringe (18.5 mm in diameter) or a small syringe (14.5 mm in diameter). It is contolled by an arduino, powered by a stepper motor, and contains 6 custom 3D printed components. The limit switch mounted on the right end support automatically stops the pump when the syringe is empty and the forward and backward buttons allow for easy replacement of the syringe. All electronics are housed in a waterproof case and an LED indicator is included to show the pump status (on, paused, and empty). 

## 3D Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a489decdc41ba192e9?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

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
| Limit Switch | 1 | End-of-travel detection |
| Aluminum Extrusion | 1 | Structural support & mount |
| M5 Machine Screws | 12 | Case assembly |
| M5 Heat Set Inserts | 12 | Case assembly |

## Custom 3D Printed Components

| Component | Material | Purpose |
|-----------|----------|---------|
| Motor Mount | ABS | Houses motor, couplings, and bearings |
| Lead screw support | ABS | Holds left end of linear rod |
| Carriage | ABS | Holds syringe plunger and moves along lead screw |
| Left End Support | ABS | Supports syringe body and bearings |
| Right End Support | ABS | Holds syringe tip |
| Case | PLA | Houses electronics |
| Case Top | PLA | Secures aluminum extrusion |

## Arduino Code

The arduino code controls the syringe pump’s flow rate, LED indicators, and forward/backward movement. The code used can be found [here](https://github.com/allihoying/syringe_code/blob/main/Ardunio_code). 

## Operating Instructions

1. Plug in the power supply  
2. In the arduino code, set the flow rate and syringe diameter variables to the desired values  
3. Plug the arduino into a computer and upload the code  
4. Load the syringe into the pump (the forward and backward buttons can be used to move the carriage into the correct position to fit the syringe)  
5. Press the power button to start the pump  
6. Press the power button again to pause the pump  
7. Watch the LED indicator to see the pump status. It will be green while running, yellow while paused, and red when empty. 

## Gallery

{% include gallery caption="3D render and final product" %}
