---
layout: page
title: Human interactive Robotics
description: Using natural language to correct robot paths
img: assets/img/6.jpg
importance: 1
category: work
---
Robotic systems are increasingly used across industrial automation, service robotics, and autonomous systems, requiring **efficient trajectory generation and adaptation**. Traditional trajectory planning methods, such as Rapidly-Exploring Random Trees (RRT) and A*, lack adaptability, while Learning from Demonstrations (LfD) enables robots to learn from human demonstrations but struggles with generalization.



## Can you chat with your robot and make it do what you want?
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/jackal_2.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=false %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/kuka_1.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=false %}
    </div>
</div>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/drone_left_right.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=false %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/drone_spiral.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=false%}
    </div>
</div>
<div class="caption">
    Instruct your robot to incorporate your preferences.
</div>

### **What is OVITA?**  
OVITA is a novel **trajectory adaptation framework** that allows users to modify robotic paths dynamically through **natural language instructions**, eliminating the need for manual reprogramming or additional demonstrations.
<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/ovita/intro.png" title="methodology" class="img-fluid rounded z-depth-1" %}
    </div>
</div>



## **Key Features**
- **LLM-Powered Adaptation**: Uses pre-trained Large Language Models (LLMs) to interpret open-vocabulary user instructions for trajectory refinement.  
- **Flexible Command Understanding**: Supports  
  - **Numerical adjustments** (e.g., *"Move left by 0.2m"*)  
  - **Abstract modifications** (e.g., *"Move in a spiral"*)  
  - **Multi-step commands** in a single instruction  (e.g., *"Go left for first 10 steps, right for next 10 and so on"*) 
- **Real-Time Interaction**: Enables iterative user feedback for refining robot actions.  

## **Methodology**

Our approach enables **dynamic trajectory adaptation** by leveraging **Large Language Models (LLMs)** to modify robot paths based on user instructions and environmental context.

#### 1. High-Level Planning & Code Generation
- The **LLM interprets user commands** (e.g., "Slow down near the person") and generates a **High-Level Plan (HLP)** outlining key trajectory modifications.
- Python code is **automatically generated** to adjust the initial trajectory.

#### 2. Code Explanation & User Interaction
- The **LLM explains the generated code** in simple terms, allowing users to understand modifications and provide feedback.
- Users can review key parameters and suggest refinements for improved adaptation.

#### 3. Execution & Constraint Satisfaction
- The modified trajectory is executed within a **Constraint Satisfaction Module (CSM)** to ensure collision avoidance, reachability, and other constraints.
- A visualization module compares the original and modified trajectories, enabling users to assess the changes.

#### 4. Iterative User Feedback
- Users can review and refine trajectory modifications through an interactive feedback loop.

## **Results**
OVITA outperforms existing approaches while provding more diverse control over robot paths.
<div class="row justify-content-sm-center">
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/ovita/results.png" title="results" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

This method ensures **real-time, user-driven trajectory adaptation**, making robot path planning **intuitive, interpretable, and highly flexible**.


{% raw %}

{% endraw %}
