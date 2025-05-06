---
layout: post
title: A Research Intern Guide
description: Some general tips and tools to make best out of your research intern. Intended for HiRo lab IISc summer interns
date: 2025-05-06
featured: true
authors:
  - name: Anurag Maurya
    affiliations:
      name: RBCCPS, IISc Bangalore

---

# 🌟 The Research Intern Guide

Congrats on making it to HiRo Lab, IISc. You're officially a research intern now. Sounds fancy. This is a short and simple guide to help you survive (and hopefully enjoy) your time here. For the next few days, I hope you’ll learn tons of new things and some life lessons ;)

---

You might be thinking that in the next few months, you’ll be working on some very cool and fancy robotics research problems—but you won’t be. Why? Because research is often boring. Most interns, when they begin working on their first research problems, have a very glorified view of what research looks like. This guide is an attempt to give you a more realistic view of how research actually works and what matters. It will show you how to spend the next few weeks and get the most out of them.

## ✍️ Some general tips:

Here are some points that, if you truly understand, will make your life much easier:

- You can contribute as a research intern in two primary ways:
    1. **Working alongside a project advisor** (e.g., a PhD student). In this case, you’ll get plenty of guidance and mostly be expected to code and perform experiments to test a methodology or hypothesis provided by your advisor. This is a great way to start and is highly recommended if you haven’t done research before.
    2. **Leading a research project yourself.** This means identifying a problem statement, reviewing the state-of-the-art (SOTA), pinpointing key issues, discussing potential solutions with your professor, forming hypotheses, conducting experiments, refining your approach, and repeating the process until you achieve good results. This path takes time—probably 5–6 months—but it will teach you how to do research more independently. You’ll learn to think on your own and pick up things that courses don’t teach, like creatively designing solutions that align with specific problems. **You need to be very patient if you decide to go with this approach.**
- **You don’t need to be a prodigy in the field you’re researching**. Research requires patience and perseverance. Rome wasn’t built in a day—and neither will your dream paper be. Commit to what you’re doing, and time will prove it was worth it.
- Before doing good research, **understand what good research looks like.** Read relevant papers. Understand not just the methodology but also the underlying motivation behind the work.
- To create new methodologies, you must first understand existing ones. Keep a strong focus on the problem you are trying to solve. “**Research without impact is just an intellectual exercise.**”-Someone said this, I don’t remember who.
- Don’t be afraid to do the "dirty work." **Indulge with hardware.** Robotics is about understanding systems—from problems in the environment down to each small part of the robot. Working with hardware is one of the best ways to develop your debugging skills.
- Don’t mistake using a tool to solve a problem for making a research contribution. A real contribution is well-designed, thoroughly studied, and explained end-to-end. It’s also important to know which approach is appropriate for which problem. For example, reinforcement learning (RL) might sound cool, but you have to ask yourself: *Is RL actually needed here?*
- Whatever you learned in your courses was just a foundation for solving problems. Now’s the time to learn new tools. Build systems that work beyond a Jupyter Notebook. **An engineer who doesn’t learn to automate effectively isn’t much of an engineer**.
- If you're working on a data-driven method, start by understanding the data. Spend weeks identifying which features matter. Analyze what salient properties of the data can be leveraged to solve the problem. This step will guide your solution. Remember: for data-based work, *garbage in = garbage out*.
- Write good code. Document and organize it well to serve two key purposes:
    - It should be easy to debug and modify. Use OOP principles to structure your code. If something is reusable, write a function or class. Use clear naming conventions.
    - In addition to the saying, “Rome wasn’t built in a day,” remember: “Rome also wasn’t built by one person.” Your code should be easy for others to run. Reproducible research ensures that others can build upon your work, and future collaborators can quickly get started. Otherwise, everything resets to ground zero.
- If you’re working in machine learning, learn **PyTorch.** Learn it by heart.[LINK:](https://pytorch.org/get-started/locally/). Most research projects rely on Torch, and you’re encouraged to use it as well.
    

---

## 🛠️ Tools You Should Be Using:



1. **GitHub:** This one’s a no-brainer. But if you’re new to it, here’s a comprehensive tutorial covering everything from basics to advanced use: [Git & GitHub Tutorial](https://medium.com/@sachinsoni600517/complete-tutorial-of-git-and-github-for-basic-to-advanced-1dd34d12b90b)
2. **ipdb:** An interactive Python debugger that’s incredibly useful for both understanding unfamiliar codebases and debugging your own code. I highly recommend it. Get started with this simple guide: [Beginner’s Guide to ipdb](https://medium.com/@lindata/a-beginners-guide-to-debugging-with-ipdb-set-trace-3d44f079f871)
3. **Weights & Biases (wandb):** If you're training ML models, wandb is essential for tracking experiments. It helps visualize training progress, manage artifacts, and compare runs easily. **Start here:** [wandb Tutorials](https://docs.wandb.ai/tutorials/)
4. **Conda:** Great for managing multiple environments without conflicts. Whether you’re working on different projects or switching between Python versions, Conda keeps everything organized. **Guide:** [Getting Started with Conda](https://docs.conda.io/projects/conda/en/stable/user-guide/getting-started.html)
5. **Notion:** A powerful tool for documentation and organization. If you haven’t used it, you should. [Check it out here](https://www.notion.com/). You can’t explain everything to your supervisor in one meeting—clear documentation helps you communicate better and track what matters. When you revisit a project after months, well-kept notes will save you from getting lost.
6. **WSL:** If you aren’t using Linux as a native install or through dual boot. Always prefer Linux over WSL. [https://learn.microsoft.com/en-us/windows/wsl/install](https://learn.microsoft.com/en-us/windows/wsl/install)
7. **ROS:** Learn the basics of ROS and ROS2, though the use of ROS has been discontinued in support of ROS2, most of the research work is still in ROS. Make use of both. **ROS1**: https://www.ros.org/blog/getting-started/, **ROS2:**  [https://docs.ros.org/en/foxy/Tutorials.html](https://docs.ros.org/en/foxy/Tutorials.html) 

> 📌If you find all this overwhelming, just know at a higher level about these tools and what problems they solve. Use whenever you encounter them. However, I believe the first 5 are a must for any kind of project.

---

## 🌱 Not necessary, but good to know:

1. **Docker:**: Containerize and share environments effortlessly. [LINK](https://waltercode.medium.com/in-depth-docker-faa0c4dd9a63)
2. **Pylint:**: Make your code cleaner and more readable. [LINK](https://pylint.readthedocs.io/en/latest/)
3. **Argparse:**: Turn your scripts into command-line tools. [LINK](https://docs.python.org/3/library/argparse.html)
4. **ThinLinc:**: For remote GUI access to Linux desktops. [LINK](https://www.cendio.com/thinlinc/how-to-get-started/)
5. **Tmux:**: Terminal multiplexing made powerful. [LINK](https://github.com/tmux/tmux/wiki)
6. **Pytest:** :  For writing effective, repeatable tests. [LINK](https://docs.pytest.org/en/stable/)
7. **Streamlit**: For building quick interactive GUIs. [LINK](https://streamlit.io/) 
