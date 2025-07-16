---
name: Theo Jansen Autonomous Robot
tools: [Mechanism Design, Lane Detection, Cascade Classifier]
image: "/assets/img/theojansen.png"
description: Designed and Developed Autonomous Legged Robot using Theo Jansen Linkage
section: undergraduate-projects
---

## Autonomous Legged Robot using Theo Jansen Linkage
### ㅤ

As a part of a robot project during my undergraduate course, I made a Theo Jansen linkage-based legged robot and participated in a self-driving challenge. I designed the linkage using simulation, fabricated the robot by myself and programmed the software for the challenge.
### ㅤ

### 1. Simulation and Modeling of Jansen Mechanism

Using V-REP Simulation, I modelled different types of linkage that can be used for a legged robot and did parameter studies in different leg, motor and frame properties.

<iframe
  width="100%" height="400"
  src="https://www.youtube.com/embed/1yakNY1jaRg?si=yN4dxsv4NL9vaxbXautoplay=1&mute=1"
  frameborder="0" allow="autoplay; encrypted-media" allowfullscreen>
</iframe>

I found the possible best case of parameters and designed the leg mechanism according to it. And using carbon rods for the legs axes and FDM printed parts, I assembled the robot.
<img src="/assets/img/jansendesign.png" alt="Robot-design" style="width:100%;">

### ㅤ
### 2. Self-Driving Algorithm using Lane and Obstacle detection
Using the legged robot, I designed Self-Driving Algorithm using Lane and Obstacle detection using Python OpenCV and Cascade Classifier.