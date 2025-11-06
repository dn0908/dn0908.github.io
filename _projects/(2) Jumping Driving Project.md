---
name: Quasi-Direct-Drive Jumping Robot
tools: [Hybrid Locomotion, Mobile Robot, Hardware Design, ROS2]
image: "/assets/img/qdd.png"
description: Continuous Jump Enabled cm-Scale Wheeled Mobile Robot
section: graduate-research
---

(This project is currently under preparation for publication and patent registration; therefore, some robot-related materials cannot be disclosed. Please email me for further information!)
###### ㅤ
## Quasi-Direct-Drive Jumping Robot 
###### ㅤ
During my graduate research at Biorobotics Lab SNU, we developed an quasi-direct-drive jumping robot that is able to drive with two wheels and jumps over a meter. This robot utilises a single direct-drive actuator for jumping, and differential driving for wheeled locomotion.
<img src="/assets/img/qdd_frame.jpg" alt="JumpingRobot-framecap" style="width:65%;">
###### ㅤ
### **What I Did :**
##### **1. Hardware Design**
I designed the jumping module part and custom controller board of the robot. The jumping module part contains rack&pinion mechanism for quasi-direct actuation and the custom controller is ARM Cortex-M7 MCU-based board.
###### ㅤ
##### **2. Control Implementation**
I integrated a Jetson Orin–MCU hierarchical control system on a ROS2 framework, linking the upper and lower controllers via UART communication. I implemented BLDC motor control, IMU filtering, and a two-wheel driving controller, and designed an impedance control strategy to mitigate landing impact. Currently, I am developing an LQR-based attitude stabilization controller to refine a fully integrated simulation–embedded–experimental control system.
<img src="/assets/img/qdd_sim.png" alt="JumpingRobot-Simexample" style="width:80%;">