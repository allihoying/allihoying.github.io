---
title: "Lightweight Generative Design Hook"
excerpt: "Lightweight hanging hook cabable of supporting 50 lbs"
header:
  image: assets/img/Syringe_pump.jpg
  teaser: assets/img/render syringe pump.jpg
gallery:
  - image_path: assets/img/Syringe_pump.jpg
  - image_path: assets/img/render syringe pump.jpg
   
---

## Overview

The generative design hook was designed to screw unto the underside of a desk or cabinet and hold objects that weigh up to 50 lbs. Hooks such as these are useful for applications such as handing bags from the underside of a desk, which can alleviate space on the desktop while maintaining legroom under the desk. These hooks can also be used in the kitchen setting in smaller spaces since mugs often take up a disproportionately large amount of cabinet space. This project idea came to me since I collect mugs, but they're all different shapes and sizes, making them unstackable. With my limited cabinet space in a small apartment, I often have a hard time finding space for everything and it would be helpful to be able to hang the mugs from the underside of the cabinet. However, the hook must be as lightweight as possible in order to minimize the load placed on the bottom of the cabinet. 

## Preserve and Obstacle Geometry

Preserve: 

* Two 8 inch diameter holes for M5 wood screws  
* A one inch diameter arc compatible with most bag and mug handles

Obstacle:

* Large plank shape directly above the screw holes, which represents the underside of a desk or a cabinet  
* 2 cylinders above the M5 screw holes, which provide a tool clearance for the wood screws  
* Circular shape filling the arc, which ensures that no material fills the space that the bag or mug handle will sit in  
* 2 side panels on either side of the hook, which ensure that the hook doesn't become too wide to fit inside of a mug handle  
* One front panel, which ensures that the user can easily reach under the screw holes and gain access to the front of the hook

## Load Case Application and Structural Constraints

4 forces were applied to the generative design study. The first force applied was a bearing force on the non fixed screw hole. The force had a magnitude of 222N, since the screw will place an equal force to the weight of the bag on the edges of the screw hole. The next force applied was a weight force pointing straight down from the bottom of the hook, which represents the maximum weight of the object hanging from the hook. The third force applied was a moment parallel to the screw holes, which was also applied to the hook. This moment represents the force the hook undergoes when the bag is placed harshly against the back of the hook, causing it to want to swing backwards. This moment was also proportional to the maximum weight of the object (222N). Finally, a gravitational force was applied pointing straight down. A fixed structural constraint was placed on the other screw hole without the bearing force applied, since a fixed constraint causes the generative design to ignore all loads applied to that geometry. This choice caused much more material to be added onto the screw hole with the bearing force, however the design should still be stable since screws will be placed in both holes, balancing the hook. The prototype can be tested further to refine the loads by using tools such as a bag weigher and measuring the amount of force that can be applied to different sections of the hook before it fractures. This method was used to prove that the hook can withstand 50 lbs (222N) when it is applied directly perpendicular to the screw holes, but the device could further be tested at different angles and locations on the hook. 

## Generative design critique

Generative design was useful for creating complex geometries quickly. It would be significantly more difficult and time consuming to calculate load paths and determine which areas of the geometry need more structural support without the help of generative design. However, there is a large learning curve when using generative design, since it requires the designer to change their way of thinking and only create obstacle and preserve geometries rather than designing the entire part from scratch. The one major limitation that I found was that fixed geometries cannot have loads applied to them, but a fixed geometry is needed. For this design, a bearing force could have been split between the 2 screw holes, with each hole undergoing 111 N of force rather than one hole experiencing the full 222 N of force. Being able to split this force would have made the design more realistic while also making it more consistent throughout the design. Generative design would be the most useful for creating functional parts that need to be lightweight, yet strong such as car parts or structural brackets. Generative design would be less useful for applications where the part needs to look a very specific way and would have an overwhelming amount of preserve and obstacle geometries. It would also not be useful for parts created with manufacturing techniques not conducive to creating complex geometries such as subtractive manufacturing or molding.   

## Applied Forces

| Name of Force | Magnitude | Location | Rationale |
| :---- | :---- | :---- | :---- |
| Gravity | 9.807 m/s^2 | Pointed straight down | Accurately tells fusion how forces should be applied in the design |
| Bearing Load | 222 N | Right screw hole | Represents the force screw exerts on the top plate of the hook when holding the weight of the bag |
| Moment | 222 N | Bottom of the hook parallel to the screw holes | Represents the force of the object being placed on the hook, causing the hook to want to swing backwards |
| Weight Force | 222 N | Bottom of the hook pointed in the direction of gravity | Represents the maximum weight of the object hanging from the hook (50lbs) |

## 3D Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a48bf3b11b8c7c97be?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Gallery

{% include gallery caption="3D render and final product" %}

