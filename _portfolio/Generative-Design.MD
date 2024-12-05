---
title: "Generative Design Skateboard Truck Hanger and Motor Mount"
excerpt: "An SLS printed skateboard hanger using Fusion's generative design feature"
header:
  image: /assets/img/mount.jpg
  teaser: /assets/img/mount.jpg
gallery:
  - image_path: assets/img/mount.jpg
  - image_path: assets/img/demomount.jpg
  - image_path: assets/img/sidemount.jpg
   
---

## Project Details

* **Powder Bed Fusion & Generative Design** 
* **Case Study**
* **Load Cases** 
* **Generative Design Critiques** 
One of the drawbacks is the high level of attention to detail needed when assigning the obstacle and preserve geometries. For example, I should have selected the entire motor as an obstacle geometry, but instead I only made the motor shaft and mounting obstacles. I was so concerned about selecting too many obstacles and over constraining the model that I missed this obstacle. This caused material to build on the motor mount plate where the motor should sit in both material outcomes, causing the hanger to not properly fit. Unfortunately, I caught this mistake after I had powder-printed my aluminum outcome hanger. If I had used a method like top down modeling using as-built joints to build the hanger myself from the parts present, I probably would have caught this issue. I also could have utilized more of the CAD modeling features to test this out before printing too, but unfortunately didn’t think of this prior to printing. While this design would work for the truck hanger portion, it does not properly mount the motor. After I printed the initial model, I went back into Fusion and updated the CAD to function properly.
Another drawback is the time needed to generate the models due to the computational intensity. By the time it takes to generate all the obstacle geometries, it almost makes more sense to create the model normally. Additionally, the organic shapes that are generated are also not compatible with traditional manufacturing techniques.

* I think generative design is useful in creating organic, creative models. The generative design outcomes are good starting points for new concepts for a design, but often require some tweaking after. It is really useful in minimizing mass while accounting for all the load cases, which is really important in applications with a high emphasis on mechanical properties. A lightweight part is arguably the biggest benefit. It’s a very powerful tool, but requires a lot of thinking to get it to work the intended way. Perhaps in a less complicated set-up, placing the constraints for the design would have been more straightforward. I think this functionality would be useful in creating fun models focused more on aesthetics than mechanical properties. 

* While I see how generative design would be useful in complicated applications that require constraints on the mass, I think it would require a very thorough understanding of physics and a complex analysis. In high-budget applications with industry experts, this tool could be very helpful in a multitude of areas. Some industries that would benefit from generative design are the automotive and aerospace industries, where product performance often improves with minimized masses. I could also see generative design being useful for its aesthetics, as the organic shapes simply look cool.For this project, I made many design choices based on the rubric on Brightspace, which provided helpful guidelines but probably limited my creativity and thinking. My main concern was hitting the items on the rubric, as opposed to thinking through all of the various design considerations on my own.



## ALSi10mg Outcome
* CAD Model: ALSi10Mg Outcome (printed)
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a48cf4791ffd4f3b47?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

* CAD Model: ALSi10mg Rendering
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4e9b4633c24622f65?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Nylon 12 Outcome
* CAD Model: Nylon 12 Outcome 
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a48612843b4eeba2c2?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


{% include gallery caption="Skateboard Truck Hanger and Motor Mount Device Gallery" %}
