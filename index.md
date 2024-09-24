
<div style="text-align: center; font-size: 24px; margin-bottom: 10px; font-weight: bold; line-height: 1.4;">
        Benchmarking Vision-Based Object Tracking for USVs in Complex Maritime Environments
</div>
<div style="text-align: center; font-size: 16px; margin-bottom: 10px; line-height: 1.4;">
    Muhayy Ud Din, Ahsan B. Bakht, Waseem Akram, Lakmal Seneviratne, and Irfan Hussain
</div>
<div style="text-align: center;">
  {% include button.html text="GitHub" icon="github" link="https://github.com/Muhayyuddin/vision-tracking" color="#0366d6" %}
  {% include button.html text="Preprint" icon="assets/arxiv.png" link="https://arxiv.org/" color="#0366d6"  %}
  {% include button.html text="FAQs"  link="#faqs" color="#0366d6"  %}
</div>
<h5 style="margin-bottom: 10px;"> Overview </h5>
<div style="text-align: justify; font-size: 14px; margin-bottom: 10px; line-height: 1.4;">
   Vision-based target tracking is crucial for unmanned surface vehicles to perform tasks such as
inspection, monitoring, and surveillance. However, real-time tracking in complex maritime environments is
challenging due to dynamic camera movement, low visibility, and scale variation. Typically, object detection
methods combined with filtering techniques are commonly used for tracking, but they often lack robustness,
particularly in the presence of camera motion and missed detections. Although advanced tracking methods
have been proposed recently, their application in maritime scenarios is limited. To address this gap, this
study proposes a vision-guided object tracking framework for USVs, integrating state-of-the-art tracking
algorithms with low-level control systems to enable precise tracking in dynamic maritime environments.
We benchmarked the performance of seven distinct trackers, developed using advanced deep learning
techniques such as Siames Networks and Transformers, by evaluating them on both simulated and real-world
maritime datasets. In addition, we evaluated the robustness of various control algorithms in conjunction
with these tracking systems. The proposed framework was validated through simulations and real-world sea
experiments, demonstrating its effectiveness in handling dynamic maritime conditions. The results show that
SeqTrack, a Transformer-based tracker, performed best in adverse conditions, such as dust storms. Among
the control algorithms evaluated, the LQR controller demonstrated the most robust and smooth control,
allowing for stable tracking of the USV.
</div>
<h5 style="margin-bottom: 10px;">Tracking results</h5> 

<video controls="" width="500" height="300" muted="" loop="" autoplay="">
<source src="https://github.com/Muhayyuddin/tracking/raw/main/video/tracking.mp4" type="video/mp4">
</video>

<video controls="" width="500" height="300" muted="" loop="" autoplay="">
<source src="https://github.com/Muhayyuddin/tracking/raw/refs/heads/main/video/circle.mp4" type="video/mp4">
</video>

<h6 style="margin-bottom: 5px;">Trackers performance</h6>
<div style="text-align: justify; font-size: 14px; line-height: 1.4;">
    We evaluated the performance of the trackers under varying conditions, including clear sea environments and dust storms. The results are showcased in the videos below.
</div>
<video controls="" width="500" height="500" muted="" loop="" autoplay="">
<source src="https://github.com/Muhayyuddin/tracking/raw/refs/heads/main/video/trackers.mp4" type="video/mp4">
</video>
<div style="text-align: justify; font-size: 14px; line-height: 1.4;">
    Trackers performance on real data.
</div>
<div style="text-align: center;">
  <img src="assets/Combined_Real.png" alt="framework" />
</div>

<h5 style="margin-bottom: 10px;">Tracking Framework</h5>
<div style="text-align: justify; font-size: 14px; line-height: 1.4;">
We proposed a vision-guided object tracking framework for USVs, integrating state-of-the-art tracking
algorithms with low-level control systems to enable precise tracking in dynamic maritime environments. The framework is composed of three main modules: the Perception
module, which incorporates sensors for environmental perception and state estimation; the Guidance module, which includes a vision-based tracker and computes
guidance commands based on pixel and distance errors; and the Control module, which integrates surge and yaw control to generate tracking commands that drive
the USV’s thrusters, enabling precise target tracking.
</div>
<div style="text-align: center;">
  <img src="assets/framework-1.png" alt="framework" />
</div>

<h5 style="margin-bottom: 10px;">Controller Tunning and Performance</h5>
<div style="text-align: justify; font-size: 14px; line-height: 1.4;">
    The animation below illustrates how different controllers work to minimize yaw error over time.
</div>
<div style="text-align: center;">
  <img src="assets/yaw_error_animation.gif" alt="Yaw Error Simulation" />
</div>
<div style="text-align: justify; font-size: 14px; line-height: 1.4;">
    The controllers performance in thrust generation for tracking.
</div>
<div style="text-align: center;">
  <img src="assets/control.png" alt="Yaw Error Simulation" />
</div>

<h5 id="faqs" style="margin-bottom: 10px;">FAQs</h5>

-Q1- Why we choose these trackers 
-Q2- Why we choose these particular COntrollers 
-Q3- What is the benefit of this research work
