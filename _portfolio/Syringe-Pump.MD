---
title: "Syringe Pump"
excerpt: "DIY syringe pump capable of 1 ul/min to 10 ul/min flow rate"
header:
  image: /assets/img/syringepump.png
  teaser: /assets/img/syringepump.png
gallery:
  - image_path: assets/img/syringepump.png
  - image_path: assets/img/syringepumpside.png

   
---

# Features

* **Low Cost** Syringe pumps are critical for many different areas of the medical field, such as delivering intravenous therapies, delivering medications to patients in palliative care, and microfluidic applications. Despite their widespread use, the average syringe pump costs thousands of dollars. In this syringe pump, many of the components were made by using 3D printed parts, which greatly reduces the cost of materials and assembly.
* **Controlled Flow Rate** The flow rate is inputted into the Arduino program and uploaded to the board. With the push of the button, the syringe pump will dispense until the liquid is gone. Mechanically speaking, the Arduino code will tell the stepper motor a certain amount of steps per second, which will dictate how many milliliters of liquid is dispensed per minute. 
* **Compatible with Different Syringe Sizes** Depending on the size of the syringe, the syringe can be inserted into the appropriate spots on the back and front stabilizers. The front barrel stabilizer is designed to support a 20 ml syringe, but also features an interchangeable insert for the 5 ml syringe. This insert accounts for the difference in size and length of the smaller syringe and can easily be added to the main body of the front barrel stabilizer.
* **LED Light Indicator** The LED light color changes in accordance with the status of the pump. The light indicates when the pump is on and not running, on and running, and when the pump has finished dispensing. 
Find the [Arduino sketch here] (https://app.arduino.cc/sketches/4bd32564-1f35-4830-a72b-0da55bf80c51?view-mode=preview).

# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH35dfcQT936092f0e4396a787ea53f9a532?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

| Off-the-shelf Parts | 
| ------------------- | 
| Syringe             | 
| Ball Bearing        | 
| Flexible Coupler    | 
| Stepper Motor       | 
| Power Supply |
| Linear Actuator |
| Lead Screw |
| Rod |
| Wires |
| Breadboard |
| LED Light |
| Screws |
| Button |

|  3D printed Parts | 
| ---------------- |
| Interchangeable Mount |
| Front Barrel Stabilizer |
| Back Barrel Stabilizer
| Box |
| Lid to Box |
| Motor Mount |
| Plunger Holder |

# Operational Instructions
* ** Depending on the size of the syringe, the syringe is inserted into the appropriate spots on the back and front stabilizers.  The flow rate is inputted into the Arduino program and uploaded to the board. Once the button is pushed, the pump will dispense liquid in the plunger until the liquid is gone. As the motor rotates the lead screw, the nut is also rotated, which is coupled to the plunger on the syringe. As the nut traverses the screw, the plunger is pushed forward at a steady pace, which dispenses the liquid inside the syringe. The LED light changes color in accordance with the status of the pump. When the pump is initially powered on, the light is yellow and the motor is not running. Once the button is pressed, the light changes to green and the motor starts. The button can be pressed again to pause the pump, which turns the light back to yellow and stops the motor. Once the plunger has been fully discharged, the switch at the end of the pathway is triggered, stopping the motor and displaying a red light. There is one button that controls the overall function of the pump by turning it on and off.

{% include gallery caption="Syringe Pump Gallery" %}
