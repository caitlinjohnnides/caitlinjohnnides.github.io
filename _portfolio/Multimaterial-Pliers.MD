---
title: "Multimaterial Pliers"
excerpt: "3D-Printed pliers made of PLA and 95A TPU"
header:
  image: /assets/img/pliers.jpeg
  teaser: /assets/img/pliers.jpeg
gallery:
  - image_path: assets/img/pliers.jpeg
  - image_path: assets/img/infill.jpg
   
---

## Project Details

* **Print-in-Place Parts** Print-in-place parts are 3D printed parts that are functional immediately after removal from the print bed. They are unique in that no post-processing or further assembly is required, as careful attention is paid to the model design and print orientation. These models feature joints and links to enable dynamic components working together. The key to many print-in-place models is to leave negative space in between moving components, creating a gap during printing. This method is incredibly useful in prototyping, as the final model is ready after a single print. Some applications include parts with springs, hinges, chains, or gears. Models for fun, such as snakes and dragons, can have fluid motion via hinges. Another example is a box with a hinged lid. Using a rigid material, such as PLA, and a flexible material, such as TPU, works well in allowing motion within the model. When the spring component is made of the flexible material, the part can have movement while still returning to its original position when not in use.

![Pliers in Action](/assets/img/movingpliers.gif)

* **Design and Iterative Process** In these multimaterial pliers, the spring component uses 95A TPU, a flexible yet strong material which allows the pliers to close and then return to the open position when not in use. A fine balance must be maintained between flexibility and sturdiness, as the spring component must be flexible enough to allow the pliers to work while also having enough structural integrity to support the jaws and handles. The functionality and ergonomics of the pliers must also be taken into consideration. When printing the middle flexible part, various clearances were tested in order to ensure a tight fit between the rigid and flexible parts. In some iterations, stringing of the TPU caused issues with structural integrity.
* **Specifications of Pliers** ***Overall Length:*** 212mm. Measured as the total length from the tip of the jaws to the end of the handles when the pliers are open, this is the most common measurement used. 
***Jaw Length:*** 77mm. Measured from the tip of the jaw to the pivot point, this measurement shows the maximum depth the pliers can grip.
***Jaw Width:*** 64mm. Measured across the widest point of the jaws when they are open, this measurement shows the type and size of objects that can be gripped securely.
***Jaw Opening:*** 17mm. Measured from the tip of the upper jaw to the tip of the lower jaw when open to their maximum extent, this measurement determines the size of the object the pliers can handle.
***Handle Length:*** 90mm. Measured from the pivot point to the handles, this measurement indicates the amount of leverage the user will be able to attain. Larger handle lengths are generally found on heavier-duty pliers.
***Grip Span:*** 92mm. Measured from the tip of the upper handle to the tip of the lower handle when the pliers are open to their fullest extent, this measurement affects the ergonomics of the pliers, and how comfortable they are to use.
* **Print Settings** In SuperSlicer, some print settings were altered to maximize the flexibility of the spring component. Infill density was set to 13% with a rectilinear sparse fill pattern. By modifying the perimeters shell setting, the bottom solid layers and top solid layers were set to 0, providing greater flexibility. Different infill densities were tested. 

![SuperSlicer Settings](/assets/img/superslicer.png)


## CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a41046c07d61f6970e?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


{% include gallery caption="Pliers Gallery" %}
