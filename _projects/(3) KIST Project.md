---
name: Vision based Complete Blood Count Software
tools: [Computer Vision, Regression Model, Optic Simulation]
image: "/assets/img/cbc.png"
description: Corpuscular Volume Estimation Using a Small Amount of Blood via Microscope Images
section: graduate-research
---

## Vision-based Complete Blood Count(CBC) Software Development
### ㅤ

In 2022 Winter, I worked as a research intern at the Center for Healthcare Robotics in Korea Institute of Science and Technology(KIST), Seoul, South Korea. I participated in a research to develop a software that uses a microscope image of a small amount of blood, without drying the blood sample.  

<img src="/assets/img/cbc.png" alt="Detection-Modules" style="width:80%;">

From the image, in order to detect all the blood cells, we adopt a loop algorithm consist of concave point detection, ellipse fitting, and blob detection. To assess the validity and accuracy of the proposed method, an investigation is conducted to examine its correlation with the Sysmex XN-1000, a widely utilized medical reference standard; we show that the correlation coefficients are higher than 0.88, showing more correlation than the method in previous studies by comparing the estimation results.  

The project was published in [23rd International Conference on Control, Automation and Systems, ICCAS 2023 (pp. 1298-1303), IEEE Computer Society](https://doi.org/10.23919/ICCAS59377.2023.10316826).
