---
title: "Microfluidic Device"
excerpt: "DIY microfluidic pinch flow fractionation device capable of sorting 165 micron and 550 micron particles"
header:
  image: /assets/img/demolded.jpg
  teaser: /assets/img/mold.JPG
gallery:
  - image_path: assets/img/mold.JPG
  - image_path: assets/img/pouring_resin.JPG
  - image_path: assets/img/demolded.jpg

   
---

## Design Considerations

* **Background** Fluids do not behave the same way at a microscale level as they do at a macroscale level. At large scales, gravity and inertia govern how fluids act. At a small scale, surface tension is the driving force. Fluids in microchambers do not experience turbulent flow, only laminar flow. This means that there is no mixing of fluids, which can be a challenge for applications like biological assays that require mixing for binding of molecules. Mixing can be achieved through chaotic advection, where sharp corners in the device cause the fluids to fold over themselves.
* **[Sorting Geometries](https://pubs.acs.org/doi/10.1021/ac049863r)** Pinched Flow Fractionation (PFF) yields passive sorting in a microfluidic device, where a microchannel has a pinched segment with a rectangular cross-section. The width of the pinched segment and the boundary angle between the pinched and the broadened segment are very important, since particle movement is dominated by flow profiles inside the channel. For effective particle separation, the width of the particle-containing solution in the pinched segment should be smaller than the diameter of the smallest particles. A narrow pinched segment is desirable for effective separation as well, so long as the segment is not clogged with the particles. The boundary angle between the pinched and broadened segments should be 180 degrees for best performance.
* **My Design** When designing my mold, the aspect ratio was a big consideration. Tall, thin parts are likely to break off during some part of the process, so the height to cross-sectional width must be less than a 4:1 ratio. Channels were kept 4mm from the edge of the device to prevent leaking. Due to VPP printing limitations, no features can be smaller than 85um. As this device sorts particles 165 microns and 550 microns in size, the sorting geometries were designed around these parameters. Inlet and outlet channels were 2mm in width, in order to minimize clogging. The 3mm pinched segment had a width of 1mm, in order to allow laminar flow while minimizing risk of particles clogging. The boundary angle between the pinched and broadened segments was 180 degrees.
* **[Creating the Mold](https://pubs.rsc.org/en/content/articlelanding/2021/lc/d1lc00744k)** Resin prints are cytotoxic due to the inability to remove residual uncured polymers and photoinitiator compounds. Parylene is an FDA USP Class VI polymer that meets the strictest testing requirements for human plantation, so it is very biocompatible. Coating resin-printed molds with parylene would render the SLA prints biocompatible and allow these prints to serve as master molds for polydimethyl siloxane (PDMS) casting. Coated prints demold more easily and have smooth, curved features.
* **Flow Rates** Particles will align to the a side wall based on the flow rates of the two inlets. The flow rate ratio of the particle-containing inlet to the buffer inlet must be 1:6.
* **Potential Applications** Microfluidic sorters are popular among biology researchers because they operate in a very small space, eradicate the need for bulky pieces of equipment, are affordable, and require minimal sample preparation. Given these benefits, microfluidic sorters enable lab-on-a-chip devices for cellular sorting, analysis, and experimental processing. Any lab that does cell research could use microfluidic sorters for these benefits. Cell sorting could also be used in diagnostics. 


## CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a407be4bb008a65e9e?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


## Instructions: From 3D printed mold to the final device
* **Print and Cure Mold** After designing a mold, SLA printing will be used to resin print the mold. The bottom of the mold, which will contact the glass slide, must be perfectly flat, so the surface needs to be parallel to the resin vat in order to avoid layer lines. During post processing, the device must be dried upside down at a slight angle before curing, in order to ensure that there is no IPA pooling. Any glossy areas are a sign of uncured resin, which will inhibit PDMS crosslinking. Be sure to not touch the inside of the mold, as any imperfections will cause sealing issues. In a fume hood, use compressed air to blow any debris out of the device. Only cure the model for 60s, as curing for too long will cause warping and no robust mechanical properties are needed.
* **Parylene Device** Depositing a thin layer of parylene, a polymer commonly used for medical device applications, will make the 3D print biocompatible and allow it to be used as a mold for PDMS casting. Coated prints have smooth features that enable easier demolding.
* **Cast PDMS** Mix PDMS elastomer and curing agent at a weight ratio of 10 : 1, and pour this solution into the print. Degas the mixture in a vacuum chamber for 30 minutes and cure in an oven at 80 °C for 3 hours.
* **Plasma Bond Glass Slide** After demolding, the PDMS devices will be bonded to glass coverslips using a PlasmaFlo PDC-FMG plasma cleaner and sterilized in an autoclave prior to use.


{% include gallery caption="Microfluidic Device Gallery" %}
