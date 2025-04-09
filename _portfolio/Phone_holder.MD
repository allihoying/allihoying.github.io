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

## Top Down Modeling

Top down modeling allows multi-component assemblies to be fully built in the correct place. This ensures that all parts fit together correctly and allows you to visualize how the final model will look during the building process. By sketching and building new components in the place where they belong, this also allows you to eliminate the assembly step later in the design process. Joints such as rigid, revolute, slider, and many more can all be used in top down modeling. As long as the correct component is activated when creating new sketches, top down modeling can be an efficient and useful method for creating multi-component assemblies. This bike phone holder is composed of 9 total components, the bike handlebars, the bottom clasp, the handle attachment, the ball bearing, the spring, the detent rotator, the top plate, the phone case, and the phone. The first component created was the bike handlebar and everything else was built based on those measurements. 

## Design Rationale

The rotation mechanism used in this project was a detent mechanism. This mechanism works by placing a ball bearing mounted on a spring in a stationary part of the assembly. Then, a circular rotating piece with several cutouts approximately the same size as the ball bearing is placed next to the ball bearing. The ball bearing should sit nested in one of the cutouts until the user rotates the circular piece. This rotation will compress the spring and allow the ball bearing to snap into the next cutout. The detent rotator in this assembly has 8 cutouts, allowing the phone to rotate every 45 degrees. Due to the 3D printing process, the stationary cutout for the ball and spring was made slightly larger than necessary to ensure that the ball would fit. Further, the small shaft meant to hold the spring in place was made slightly smaller than necessary in order to ensure that it would fit within the diameter of the spring. In the future, a larger ball bearing would be used to allow the ball to snap into the cutouts more easily. While the detent mechanism did work, it was not as stable as I would have liked it to be. With a thicker spring and a larger ball bearing, the rotator could shift more easily and be stable when in the correct position. 

These parts were created using FFF printing so that multiple iterations could easily be printed and the part could be optimized. The bottom clasp, the detent rotator, and the top plate were all printed in PLA, while the phone case was printed in TPU. The PLA was used so that the parts would be rigid and stable, while TPU was used to allow the phone case to bend around the phone easily. 

## 3D Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4bacc05d0ce550897?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


## Assembly and Operating Instructions

1. Place spring on the shaft in the stationary part of the detent mechanism
2. Place ball bearing on top of the spring
3. Place the detent rotator on top of the stationary part with the ball bearing nested in one of the cutouts
4. Add heat sink inserts into the stationary part
5. Screw the top plate into the stationary part using M5 bolts 
6. Attempt to rotate the mechanism and loosen the bolts if necessary to allow the rotator to move more easily
7. Snap the phone case onto the top of the rotating mechanism
8. Place the assembly onto the bike handle and screw the bottom clasp onto the other side using 4 M5 bolts and nuts
9. Put phone into the phone case and rotate into the desired position

## Gallery

{% include gallery caption="3D render and final product" %}
