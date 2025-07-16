---
name: Unmanned Water Rescue Robot
tools: [Mechanism Design, Emergency Detection]
image: "/assets/img/resq4u.png"
description: Designed and Developed Unmanned Water Rescue Robot using Emergency Detection
section: undergraduate-projects
---
## Unmanned Water Rescue Robot : ResQ4u
### ㅤ
During my undergraduate project, I developed an unmanned water rescue robot. The robot system autonomously detects emergency situation and precisely throws the self-inflating rescue tube to the target. This system was awarded several times and was also published in [Trans. Korean Soc. Mech. Eng. C](https://doi.org/10.3795/KSME-C.2024.12.2.057)!


<div style="display: flex; justify-content: center; align-items: center; gap: 20px; flex-wrap: wrap;">

  <!-- Image -->
  <img src="/assets/img/resq4uoverview.png" alt="Project-introduction" style="width: 60%; min-width: 250px;">

  <!-- Video -->
  <iframe
    width="35%" height="160"
    src="https://www.youtube.com/embed/03CUmIzoZ04?si=J2b-9uis-7GliLWH"
    frameborder="0" allow="autoplay; encrypted-media" allowfullscreen>
  </iframe>

</div>

### ㅤ
### 1. Autonomous Emergency Detection
The presented system integrates an IR camera, a LiDAR, and an object detection machine learning model for effective detection in night and unpopulated environments.
<img src="/assets/img/emergencydetection.png" alt="Detection-Modules" style="width:80%;">

The model trained to continuously operate within the camera frame to detect whether a person has fallen into the water. A Single Shot Detector (SSD) object detection model is used, with a convolutional neural network-based MobileNet as the backbone, achieving fast object detection optimized for mobile devices.

A sliding window-based algorithm is additionally applied to track detected rescue situations. By using a day/night camera module equipped with an IR-cut filter, the model’s performance was validated under both daytime and nighttime conditions.

### ㅤ
### 2. Targeting Mechanism & Algorithm
<img src="/assets/img/pantiltmech.png" alt="Pantilt-mechanism" style="width:80%;">
The overall frame was designed to allow left/right rotation of both the launching and detection modules, as well as additional up/down rotation specifically for the detection module. For horizontal rotation, a mechanism based on a large turntable principle was designed, using a stepper motor, caster wheels, ball bearings, and aluminum profiles to support heavy loads and enable smooth rotation.

### ㅤ
### 3. Automatic Launching Mechanism Design
<img src="/assets/img/pitchingmachine.png" alt="Launcher-mechanism" style="width:80%;">
To accurately launch the resque tube to the target, we designed quasi-direct-drive launching mechanism similar to a baseball pitching machine. The motor velocity was mapped to the thrown distance of the tube by multiple experiments, thus launching distance control was available.

<iframe
  width="100%" height="400"
  src="https://www.youtube.com/embed/qVO7ZP8KgL4?si=mrC7ZubSV2nPYvvFautoplay=1&mute=1"
  frameborder="0" allow="autoplay; encrypted-media" allowfullscreen>
</iframe>

The PFD is normally stored in a compartment for reloading. During launch, it is inserted into the launching device via a linear guide. As the PFD is fed, it is partially compressed and passes between the two wheels, and upon passing through, it is propelled forward by the frictional force. After launch, the platform moves backward so that the next PFD stored above drops into position on the platform. This reloading mechanism allows the system to operate fully autonomously without human intervention.