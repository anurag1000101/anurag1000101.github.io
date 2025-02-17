---
layout: page
title: RRC intern
description: video object detection on BDD100K
img: assets/img/3.jpg
importance: 2
category: work
---

This project focuses on detecting objects in driving videos under challenging weather conditions using **temporal aggregation techniques**.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/vodta_1.png" title="method" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
Predictions on blurred real-world data from BDD100k dataset
</div>

## Methods & Benchmarks

- **Fine-tuning Faster R-CNN**:
  - The Faster R-CNN model was fine-tuned on the **BDD100K** dataset to improve detection in **adverse weather** and **lighting** conditions.
  - Used Detectron2 framework. [LINK](https://github.com/facebookresearch/detectron2)

- **Temporal Keyframe Matching**:
  - **Windowed Hungarian Algorithm** (No-Learning) for object tracking.
  - **LightGlue** (No-Learning) for feature matching.
  
- **Faster R-CNN Benchmarking**:
  - Benchmarking was conducted to compare performance against standard models and evaluate improvements.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include video.liquid path="assets/video/bdd100k_short.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=false %}
    </div>
</div>

## Goal
The primary goal of this project is to **improve object detection accuracy** in real-world driving scenarios without adding complex learning.


{% raw %}

{% endraw %}