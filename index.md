---
title: 
feature_text: |
feature_image: "assets/scaled_USV_m.png"
excerpt: Here we will add the description of the paper
---
<div style="text-align: center; font-size: 24px; font-weight: bold; line-height: 1.4;">
        Benchmarking Vision-Based Object Tracking for USVs in Complex Maritime Environments
</div>
<div style="text-align: center; font-size: 16px; line-height: 1.4;">
    Muhayy Ud Din, Ahsan B. Bakht, Waseem Akram, Lakmal Seneviratne, and Irfan Hussain
</div>
<div style="text-align: center;">
  {% include button.html text="GitHub" icon="github" link="https://github.com/daviddarnes/alembic" color="#0366d6" %}
  {% include button.html text="Preprint" icon="assets/arxiv.png" link="https://arxiv.org/" color="#0366d6"  %}
</div>

<h4>Tracking results</h4> 

<video controls="" width="500" height="300" muted="" loop="" autoplay="">
<source src="https://github.com/Muhayyuddin/tracking/raw/main/video/tracking.mp4" type="video/mp4">
</video>

<video controls="" width="500" height="300" muted="" loop="" autoplay="">
<source src="https://github.com/Muhayyuddin/tracking/raw/refs/heads/main/video/circle.mp4" type="video/mp4">
</video>

Trackers performance
<video controls="" width="500" height="500" muted="" loop="" autoplay="">
<source src="https://github.com/Muhayyuddin/tracking/raw/refs/heads/main/video/trackers.mp4" type="video/mp4">
</video>

<h1> Overview </h1>
<div style="text-align: justify; font-size: 14px; line-height: 1.4;">
    Vision-based target detection and tracking are crucial for Unmanned Surface Vehicles (USVs) to perform tasks such as inspection, monitoring, and surveillance. However, real-time tracking in complex maritime environments is challenging due to factors such as dynamic camera movement and changing sea conditions. Traditional object detection methods combined with filtering techniques are commonly used for tracking, but they often lack robustness, particularly in the face of camera motion and missed detections. Although advanced tracking methods have been proposed recently, their application in real-time maritime scenarios remains limited. To address this gap, this study proposes a vision-guided object tracking framework for USVs, integrating state-of-the-art tracking algorithms with low-level control systems to enable precise tracking in dynamic maritime environments. We benchmarked the performance of five distinct trackers, developed using advanced deep learning techniques such as Convolutional Neural Networks (CNNs) and Transformers, by evaluating them on both simulated and real-world maritime datasets. In addition, we evaluated the robustness of various control algorithms in conjunction with these tracking systems. The proposed framework was validated through simulations and real-world sea trials, demonstrating its effectiveness in handling dynamic maritime conditions.
</div>
<h1>Tracking Framework</h1>
<div style="text-align: center;">
  <img src="assets/framework-1.png" alt="framework" />
</div>
Add the image of the tracking framework with a short description.


<h1>Controllers</h1> 
<div style="text-align: center;">
  <img src="assets/yaw_error_animation.gif" alt="Yaw Error Simulation" />
</div>

<h1>FAQs</h1> 
-Q1- Why we choose these trackers 
-Q2- Why we choose these particular COntrollers 
-Q3- What is the benefit of this research work


