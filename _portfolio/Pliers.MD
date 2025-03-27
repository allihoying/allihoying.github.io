---
title: "Multi-Material Pliers"
excerpt: "PLA and TPU pliers capable of picking up resistors"
header:
  image: assets/img/Syringe_pump.jpg
  teaser: assets/img/render syringe pump.jpg
gallery:
  - image_path: assets/img/Syringe_pump.jpg
  - image_path: assets/img/render syringe pump.jpg
   
---

##Overview – Print in Place

The goal of this project was to create multi material needle nose pliers capable of picking up resistors using only a FFF 3D printer. The base of the pliers was created using PLA for a more sturdy grip, while TPU was used to create a flexible spring \- allowing the pliers to close and then return to the open position when relaxed. These pliers can be made using print in place technology, which requires no post processing. This can be done using an FFF printer with multiple extruders or splicing filaments in a single extruder, both of which allow multiple materials to be printed at the same time. Some applications for multi material printing and print in place technologies include creating hinges, creating helmets with padding, or creating flexible supports in robots.

For filaments to bond well together, they should have surface energy, chemical composition, shrinkage, cooling rates, and mechanical compatibility. For this application, PLA and TPU are used, but PLA can also be printed with PVA and ABS can be printed with HIPs.

##CAD

\<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4b1e4dc6141f18eb7?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"\>\</iframe\>

##Design

The pliers were created using two different materials that were connected using dovetail links. When extruding in CAD, both handles, both jaws, and the flexible center piece were turned into different bodies and separately printed. The handles and jaws were printed in PLA, while the center piece was printed in TPU. After the pieces were finished, they were press fit together to form a tight connection.  

Two separate center components were printed in order to try out varying levels of flexibility. One was created using 31% infill while the other was created using 23% infill. Both were printed with a grid infill pattern and no top or bottom layers were used so that the flexibility was consistent throughout the entire spring area. Ultimately, the 31% infill center piece was used to make the pliers springier.

The handles and jaws were changed multiple times in CAD to create the appropriate shape and grip to pick up small resistors. The gap between the jaws in the open position was originally around 16 mm wide, which would not have been compatible with the 25 mm spring length, since this spring can only close a gap 13 mm wide. Ultimately, the gap was narrowed to only 8 mm wide, which allowed resistors to be picked up quickly. Another aspect that was changed often in the cad model was the distance between the ends of the handles. Originally, the handles were not far enough apart, so they would hit each other before the jaws of the pliers closed. In the final print, the handles were widened slightly, allowing the jaws to completely close. However, the handles were still close enough to touch each other when closed, so in future iterations this distance would be increased even more.

The final pliers the handles were set 49 mm apart, the jaws were set 8 mm apart, and the springy center component was 25 mm wide.

##Gallery

{% include gallery caption="Design Iterations" %}

##Gif
