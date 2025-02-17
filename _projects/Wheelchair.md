---
layout: page
title: Autonomous Wheelchair
description: 2D and 3D navigation of a robotic wheelchair
img:
importance: 3
category: work
---

This project enhances **autonomous wheelchair navigation** and **person detection** using **LiDAR-based perception and control algorithms**. The system recieves a goal position from the BCI headset and then shall autonomously naviagte to that goal position.

## 2D and 3D naviagtion
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/2D_nav-mute-video.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=false %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/3D_nav-mute-video.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=false %}
    </div>
</div>
<div class="caption">
    2D and 3D navigation of a wheelchair robot in a cluttered environment. The video shows the naviagtion stack along with sensor readings.
</div>

### Autonomous Navigation
- **HectorSLAM** for real-time mapping. This was chosen since it allows for map-creation without any explicit odometry.
- **AMCL** (Adaptive Monte Carlo Localization) for precise localization.  see [AMCL ROS](http://wiki.ros.org/amcl)
- **PID Control** for smooth and accurate movement of wheels on different terrains.  

### Person Detection
- **Fine-tuned DR-SPAAM** (attention-based autoregressive model) for detecting people in **2D LiDAR sequences**.
- Reference: [Person detection in 2d range data](https://github.com/VisualComputingInstitute/2D_lidar_person_detection)

## System Impact
This system ensures **safe and efficient navigation** in **dynamic environments**. 

{% raw %}

{% endraw %}