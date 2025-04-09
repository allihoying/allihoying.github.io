---
title: "Rotating Bike Phone Holder"
excerpt: "3D printed phone holder for bike handles that is capable of rotating"
header:
  image: assets/img/Renter_front.png
  teaser: assets/img/Detent_pic.png
gallery:
  - image_path: assets/img/Detent_pic.png
  - image_path: assets/img/Section_view.png
  - image_path: assets/img/render_isometric.png
  - image_path: assets/img/Renter_front.png
  - image_path: assets/img/Render_side.png
  - image_path: assets/img/Rotate_GIF.gif
   
---

## Overview

This syringe pump was created as part of Vanderbilt's rapid prototyping class. The pump is capable of delivering consistant flow rates between 1 uL / min and 10 mL / min for either a large syringe (18.5 mm in diameter) or a small syringe (14.5 mm in diameter). It is contolled by an arduino, powered by a stepper motor, and contains 6 custom 3D printed components. The limit switch mounted on the right end support automatically stops the pump when the syringe is empty and the forward and backward buttons allow for easy replacement of the syringe. All electronics are housed in a waterproof case and an LED indicator is included to show the pump status (on, paused, and empty). 

## 3D Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4bacc05d0ce550897?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


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
