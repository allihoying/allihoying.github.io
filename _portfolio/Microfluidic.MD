---
title: "Microfluidic Sorter"
excerpt: "Microfluidic device capable of separating 125-150 um particles from 425-500 um particles"
header:
  image: assets/img/Syringe_pump.jpg
  teaser: assets/img/render syringe pump.jpg
gallery:
  - image_path: assets/img/Syringe_pump.jpg
  - image_path: assets/img/render syringe pump.jpg
   
---

## Introduction

Microfluidic devices are used to test small amounts of liquids, usually blood, for disease markers. By using a small amount of liquid, the blood required from the patient and the amount of antibodies and other reagents required to test the blood is limited, leading to cheaper tests. The channels in microfluidic devices can be as small as 60 micrometers, making surface tension the dominant force effecting the fluid’s movement. This movement can be manipulated by the shape, size, and pathways of the channels, leading to either mixing or separating of specific particles

Pinch flow fractionation is one way to separate particles by size using microfluidic devices. In this method, 2 inlet channels are used – one containing particles and one without particles. These channels combine in a pinched region, which forces the particle stream against the wall and aligns all particles regardless of their size. The channel then widens again, causing the particles to separate based on their size. Larger particles are directed towards the center of the channel, while the smaller particles remain close to the wall. Outlet channels can then be strategically placed to collect particles based on size, keeping in mind that all channels must have even flow rates to maintain consistent resistance throughout every channel. To determine where outlet channels should be located, the following equation can be used:

![][image1]

Y \= Y axis height

Wp \= pinched width

Wb \= broad width

D \= particle diameter

Pinched flow fractionation in microfluidic devices can be used for many medical applications: for example, separating cancer cells from white blood cells \[1\]. Because circulating tumor cells in the blood of cancer patients can lead to the formation of new tumors in secondary sites, it would be beneficial to separate these cells out of the blood to prevent metastases formation. This method of cell separation could also be used to diagnose cancer early on if these cells are found in the blood before a tumor forms. Catching cancer early is one of the best ways to increase treatment effectiveness, so finding the cells before they form tumors could increase life expectancy of cancer patients.

## Instructions

1\.     CAD model

* Base model \= 25 mm wide by 75 mm long in order to sit flat against a microscope slide  
* Minimum feature size \= 85 um with 25 um resolution  
* Inlets and outlets \= must be 3 mm from the edge of the device and 11 mm away from each other (center to center). A 1.5 mm post extruded above the top of the mold will create a hole that is compatible with the microfluidic barb.  
* Channel size \= must be 1.2 – 1.5 times the diameter of the largest particle. The length, width, and depth of the outlet channels should be consistent to create equal resistance and flow rates.  
* Channel placement \= outlet channels should be placed at specific Y axis heights to collect each particle separately. See equation in the introduction to calculate specific heights.

2\.     Print and cure mold:

* Resin print the mold using 0.025 mm or 0.05 mm layer height  
* When printing, ensure that the bottom of the mold is flat and parallel to the resin vat  
* Wash the print for 5 minutes on the print bed and 5 minutes in fresh IPA  
* Let the device try upside down for 30 minutes, ensuring that IPA does not pool inside  
* Gently blow debris out of the channels with compressed air. Do not touch the inside of the cured mold  
* Perform a 60 second spot cure with support on  
* Remove support material

3\.     Parylene device:

* Transfer cured prints into a Labcoter parylene deposition machine  
* Coat the mold with parylene to create a hydrophobic and biocompatible barrier

4\.     Cast PDMS:

* Mix PDSM elastomer (Sylgard 184; Ellsworth Adhesive Company) and a curing agent at a 10:1 ratio  
* Pour the mixture onto the print  
* Degass for 30 minutes in a vacuum chamber  
* Cure in an oven at 80 C for 3 hours

5\.     Plasma bond glass slide:

* Bond PDSM devices to glass slides using a PlasmaFlo PDC-FMG plasma cleaner  
* Sterilize with an autoclave

## Discussion

  Parylene is an FDA USP Class VI polymer that creates a hydrophobic barrier, which is impermeable to small molecules, water, and gases. The coating preserves the integrity of devices in the body, and nanometer thick films are commonly deposited on implanted medical devices \[2\]. Resin printed molds must be coated with parylene prior to casting the PDMS since most resins are cytotoxic and cannot be used in applications involving cells. The parylene coating stops toxic material from leaching out of the 3D print and allows the devices to be used as master molds for PDMS devices. After the mold has been created, the biocompatible microfluidic device could easily be used for applications such as blood testing. If small amounts of antibodies were placed in one inlet and blood was placed in the other, a microfluidic mixer could successfully detect many different medical conditions. Microfluidic sorters could also be used for several biomedical applications such as cancer research, separating stem cells, or separating blood cells.

  The geometry of the mixer shown in this example is capable of sorting 2 different particle sizes, 125-150 um and 425-500 um. Using the equation shown in the introduction, I found that the smaller particles would end up between 16.625 mm and 17.021 mm on the Y axis. Conversely, the larger molecules would end up between 11.083 mm and 12.271 mm on the Y axis. Four outlet channels with equal cross sectional areas were used to expel the liquid and particles. However, due to spatial constraints caused by the 11 mm barbs, the lengths of the channels vary. The width the particles were able to separate (Wd) was 19 mm, as the slide was 25 mm wide with a 3 mm buffer on either side. The pinch point was 0.75 mm wide, which is 1.5x the 500 um particle size. Since resistance is limited by the smallest outlet (the 1.50 mm diameter barb exit) and the cross sectional area of each channel is the same, the flow rate through each channel should be similar. Therefore, even though the channels are different lengths, the streamlines should be consistent enough to maintain proper separation. However, to improve sorting effectiveness in the future, smaller barbs will be used to ensure that all of the channels can be the same length.

## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4d405d63c3d0f40fc?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## References

\[1\] Pødenphant, M., Ashley, N., Koprowska, K., Mir, K. U., Zalkovskij, M., Bilenberg, B., Bodmer, W., Kristensen, A., & Marie, R. (2015). Separation of cancer cells from white blood cells by pinched flow fractionation. Lab on a Chip, 15(24), 4598–4606. https://doi.org/10.1039/c5lc01014d

\[2\] O’Grady, B. J., Geuy, M. D., Kim, H., Balotin, K. M., Allchin, E. R., Florian, D. C., Bute, N. N., Scott, T. E., Lowen, G. B., Fricker, C. M., Fitzgerald, M. L., Guelcher, S. A., Wikswo, J. P., Bellan, L. M., & Lippmann, E. S. (2021). Rapid prototyping of cell culture microdevices using parylene-coated 3D prints. Lab on a Chip, 21(24), 4814–4822. https://doi.org/10.1039/d1lc00744k

[image1]: <data:image/png;base64,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>
