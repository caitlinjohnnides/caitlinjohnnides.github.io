---
title: "Generative Design Skateboard Truck Hanger and Motor Mount"
excerpt: "An SLS printed skateboard hanger using Fusion's generative design feature"
header:
  image: /assets/img/seated.JPG
  teaser: /assets/img/seated.JPG
gallery:
  - image_path: assets/img/side.JPG
  - image_path: assets/img/divot.JPG
  - image_path: assets/img/pulley.JPG
  - image_path: assets/img/bottom.JPG
  - image_path: assets/img/bottom2.JPG
  - image_path: assets/img/mounted.JPG
  - image_path: assets/img/bothmodels.JPG
   
---

## Project Details

**Powder Bed Fusion & Generative Design** 
* Powder bed fusion pairs particularly well with generative design as generative design often yields organic, hard to manufacture parts. These parts are not compatible with traditional manufacturing techniques and often traditional 3D printing techniques, due to odd overhangs and many curves. Powder bed fusion allows for the creation of the non-traditional shapes, which are often useful in reducing mass for aerospace and automotive industries. Designing a part that has to be traditionally manufactured can be limiting and potentially increase the amount of material needed.

**Case Study**
* The [Airbus A320 aircraft](https://www.airbus.com/en/newsroom/news/2016-03-pioneering-bionic-3d-printing) wall was redesigned with Autodesk’s generative design. Fixed between the passenger seating area and plane’s galley, this dividing wall will sometimes be used to support the jumpseats used by cabin crews during takeoff and landing. It needs to be strong, which with traditional materials and manufacturing processes, makes it heavy and bulky. The primary objectives were to reduce the weight of the wall, minimize the number of parts, and ensure structural integrity. This study resulted in a lighter design, fewer parts, and a lower cost.

**Load Cases** 
* Proper load cases were important as they determined how much mass was generated in order to support the applied loads. If too little forces were applied, then the truck hanger would not have weak mechanical properties and might not have been functional. A proper free body diagram of the entire setup would have improved the process.There are many scenarios where the forces might change, such as sharp turns or riders of different weights, so an algorithm that would account for these changes would improve the process. 

* I determined what forces to apply to the model by thinking through a rider on a skateboard and using ChatGPT to tell me what parameters I needed. In class, we calculated the two of the three forces on the motor mounting plate: the torque applied to the plate from the motor and the weight from the motor. I calculated the tension from the pulley. The rod experiences the weight of the rider at the middle and shear forces on each end of the rod.

| Force | Value |
|------ |-------|
| Torque on Motor Mount Plate | 296 Nmm|
| Remote Weight on Motor Mount Plate| 8.31 N |
| Remote Tension from Pulley | 200 N |
| Weight of Rider | 668 N |
|Shear Forces (one on each end of rod) | +/- 683 N | 

* I placed the structural constraint at the pivot cup. Structural constraints define the loads, supports, and other boundary conditions that the design must accommodate. This point acts as an anchor, as the design will be optimized to transfer loads to this support efficiently. If the constraint were elsewhere, then the bulk of the mass would have also generated elsewhere. I chose this point as it is the “base” of the model.

**Generative Design Critiques** 
* One of the drawbacks is the high level of attention to detail needed when assigning the obstacle and preserve geometries. For example, I should have selected the entire motor as an obstacle geometry, but instead I only made the motor shaft and mounting obstacles. I was so concerned about selecting too many obstacles and over constraining the model that I missed this obstacle. This caused material to build on the motor mount plate where the motor should sit in both material outcomes, causing the hanger to not properly fit. Unfortunately, I caught this mistake after I had powder-printed my aluminum outcome hanger. If I had used a method like top down modeling using as-built joints to build the hanger myself from the parts present, I probably would have caught this issue. I also could have utilized more of the CAD modeling features to test this out before printing too, but unfortunately didn’t think of this prior to printing. While this design would work for the truck hanger portion, it does not properly mount the motor. After I printed the initial model, I went back into Fusion and updated the CAD to function better. However, as I removed certain issues, new issues arose. For example, in the initial model I printed, there was plenty of clearance for kingpin installation (and I didn’t have an obstacle in place). In subsequent generations, material was generated to block the kingpin. However, when I added an obstacle, the model became overconstrained. In my final design, I could have added a normal cut through the center to give the proper clearance, but this would have gone against the purpose of using generative design. Also, sometimes the algorithm ignored my obstacles and generated material where I knew there was an obstacle, such as through the sleeve for the rod.
Another drawback is the time needed to generate the models due to the computational intensity. My computer also crashed multiple times during the computations (and I have a pretty new and powerful computer). By the time it takes to generate all the obstacle geometries, it almost makes more sense to create the model normally. Additionally, the organic shapes that are generated are also not compatible with traditional manufacturing techniques.

* I think generative design is useful in creating organic, creative models. The generative design outcomes are good starting points for new concepts for a design, but often require some tweaking after. It is really useful in minimizing mass while accounting for all the load cases, which is really important in applications with a high emphasis on mechanical properties. A lightweight part is arguably the biggest benefit. It’s a very powerful tool, but requires a lot of thinking to get it to work the intended way. Perhaps in a less complicated set-up, placing the constraints for the design would have been more straightforward. I think this functionality would be useful in creating fun models focused more on aesthetics than mechanical properties. 

* While I see how generative design would be useful in complicated applications that require constraints on the mass, I think it would require a very thorough understanding of physics and a complex analysis. In high-budget applications with industry experts, this tool could be very helpful in a multitude of areas. Some industries that would benefit from generative design are the automotive and aerospace industries, where product performance often improves with minimized masses. I could also see generative design being useful for its aesthetics, as the organic shapes simply look cool.For this project, I made many design choices based on the rubric on Brightspace, which provided helpful guidelines but probably limited my creativity and thinking. My main concern was hitting the items on the rubric, as opposed to thinking through all of the various design considerations on my own.


## ALSi10mg Outcome
* CAD Model: ALSi10mg Outcome #1
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a48cf4791ffd4f3b47?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

* CAD Model: ALSi10mg Outcome #2 (the model that was tested)
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4cf50a58d83c4187e?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
* ALSi10mg Renderings

Here are both printed models side by side. Note how in the first model (where no obstacle geometry for clearance around the kingpin was placed), there was sufficient room to fasten the kingpin automatically generated. 
!(Side by Side)[/assets/img/bothmodels.JPG]

In the tested model, there was enough clearance around the base for the truck to turn.
!(base)[/assets/img/base.gif)

Additionally, the distance between the two pulleys was properly calculated, allowing for a tight fit that allowed the wheels to turn.
!(wheels)[/assets/img/pulley.gif]

## Nylon 12 Outcome
* CAD Model: Nylon 12 Outcome 
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a48612843b4eeba2c2?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

* Nylon 12 Renderings

## Complete Assembly
* CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4e9b4633c24622f65?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

* Complete Renderings
!(full rendering)[/assets/img/fullrendering.jpg]
!(full rendering)[/assets/img/topview.jpg]

{% include gallery caption="Truck Hanger & Motor Mount Photo Gallery" %}

