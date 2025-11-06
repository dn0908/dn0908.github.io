---
name: Underactuated Hip Exosuit Control
tools: [Wearable, Human-in-the-loop Optimization, ROS2]
image: "/assets/img/uhe.png"
description: Ultralightweight hip assistant robot and Human-in-the-loop Control Parameter Optimization
section: graduate-research
---

(This project is currently under preparation for publication and patent registration; therefore, some robot-related materials cannot be disclosed. Please email me for further information!)
###### ㅤ
## Underactuated Hip Exosuit 
###### ㅤ
During my graduate research at Biorobotics Lab SNU, we developed an underactuated hip assistant soft wearable robot. This robot is able to assist 4 torques(Left flextion, Left extension, Right flextion, Right extension) using a single motor by differential mechanism. The Robot uses 2 IMU sensors for gait estimation and the system is integrated using ROS2.
<img src="/assets/img/uhe_overview.png" alt="UHE-Robot" style="width:80%;">
###### ㅤ
### **What I Did :**
##### **1. Lightweight Controller**
I designed a custom IO board using Raspberrypi Compute Module 5 for the robot's control. 
<img src="/assets/img/uhe_controller.png" alt="UHE-Controller" style="width:80%;">
###### ㅤ
##### **2. Human-in-the-loop Optimization**
I implemented a ROS2-based controller and applied CMA-ES–based Human-in-the-loop optimization to automatically tune assistance parameters for each user. The system connected MATLAB with the controller via wireless communication, enabling automated experiment execution and real-time metabolic cost evaluation.
<img src="/assets/img/hilo.png" alt="UHE-Hilo" style="width:80%;">