---
name: Autonomous Anomaly Detection Robot
tools: [Anomaly detection, Anomaly Classification, Multimodal deep learning, Autonomous Driving]
image: "/assets/img/batcam.png"
description: Developed a Vision-Ultrasound Robotic System based on Deep Learning for Gas and Arc Hazard Detection in Manufacturing
section: graduate-research
---
## Vision-Ultrasound Robotic System based on Deep Learning for Gas and Arc Hazard Detection in Manufacturing
### ㅤ
During my undergraduate research in the Soft Computing Lab, Yonsei University, I developed a deep learning-based robotic system to detect and classify anomaly in manufacturing environment.

The robot system mimics the human visual-acoustic reasoning process while extending its perceptual range through directional ultrasonic sensing. 

<img src="/assets/img/batcam_overview.png" alt="Robot-Overview" style="width:80%;">

### **What I Did :**
##### **1. Hardware Development**
I built a custom robot using the mobile chasis Scout mini from AgileX Robotics. A custom power circuit for the sensors and the pan-tilt actuating system for sensor manipulation was designed.

<img src="/assets/img/batcam_hw.png" alt="Robot-HW" style="width:100%;">

##### **2. Autonomous Navigation System**
I applied autonomously guided navigation algorithm by using RealSense D435i to follow the lane, identify the 2D tags installed on the field and stop when obstacle is detected. PID Controller was used for lane following and the 2D tag detection was used for robot localization. Depth data was also monitored to trigger an emergency stop if obstacles persist beyond a threshold period.

##### **3. Target Detection and Signal Enhancement**
I combined object detection model with beamforming network to locate critical components and improve ultrasonic signal quality. A 112-channel ultrasonic camera that captures sound and RGB frame in real-time was used. When a target facility is detected in the RGB frame first, the pan-tilt manipulator targets the sensor to the facility. Then the object detection model detects critical components in the facility. The detected components' center point is scanned from the ultrasonic microphone using grid search algorithm and then sound signal is beamformed for post-run analysis.
<img src="/assets/img/batcam_layout.png" alt="Robot-SWLayout" style="width:50%;">

##### **4. Deep Learning-Based Leak and Discharge Detection Model**
To detect and classify leak and discharge, the model is consisted of 3 steps: 1) STFT and Gamma Correction, 2) Inception Block Feature Extraction, 3) MLP Classification. We developed an Inception-style CNN block, designed to simultaneously capture multi-scale time-frequency features. The Inception-style CNN effectively represents complex ultrasonic patterns by employing multiple parallel convolution kernels and stacked Inception blocks for hierarchical feature extraction.

<img src="/assets/img/batcam_model.png" alt="Robot-Model" style="width:100%;">

This project is currently in preperation for publication.
You can see the preprint in arxiv!

<iframe
  width="100%" height="400"
  src="https://www.youtube.com/embed/SZWnzXeCERg?si=Jrif8x4vgX6aPRn-autoplay=1&mute=1"
  frameborder="0" allow="autoplay; encrypted-media" allowfullscreen>
</iframe>