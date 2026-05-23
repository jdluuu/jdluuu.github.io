---
layout: homepage
---

## About Me

Hi! I am currently pursuing a master's degree in the FASTLab (Fire Group) at the College of Control Science and Engineering, Zhejiang University, under the supervision of [Yanjun Cao](https://scholar.google.com/citations?user=Q44CBbgAAAAJ&hl=zh-CN) and [Chao Xu](https://scholar.google.com/citations?user=IOCO-YQAAAAJ&hl=zh-CN).

Previously, I obtained a bachelor's degree in Automation from Shandong University with the honor of Excellent graduation thesis (top 2%). 

<p class="phd-call">I'm looking for a potential PhD position in Fall 2027. Please contact me if you see a potential fit!</p>

<style>
  .phd-call {
    color: #d40000;
    font-weight: 700;
    font-size: 1.em;
    text-align: center;
    margin: 0.0em auto 1.0em;
    display: inline-block;
    width: 100%;
    transition: color 0.2s ease;
  }
  .phd-call:hover {
    animation: phd-call-shake 0.5s;
    animation-iteration-count: infinite;
  }
  @keyframes phd-call-shake {
    0%   { transform: translate(1px, 1px) rotate(0deg); }
    10%  { transform: translate(-1px, -2px) rotate(-1deg); }
    20%  { transform: translate(-3px, 0px) rotate(1deg); }
    30%  { transform: translate(3px, 2px) rotate(0deg); }
    40%  { transform: translate(1px, -1px) rotate(1deg); }
    50%  { transform: translate(-1px, 2px) rotate(-1deg); }
    60%  { transform: translate(-3px, 1px) rotate(0deg); }
    70%  { transform: translate(3px, 1px) rotate(-1deg); }
    80%  { transform: translate(-1px, -1px) rotate(1deg); }
    90%  { transform: translate(1px, 2px) rotate(0deg); }
    100% { transform: translate(1px, -2px) rotate(-1deg); }
  }
</style>

<!-- I am deeply fascinated by robotics's future and committed to advancing research in this field. If you're interested in discussing my work or potential collaborations, feel free to email me at jdlu@zju.edu.cn -->

## Research Interests
<!-- 
My research interests include multi-robot collaboration and relative localization. I am also interested in mechanical design and reinforcement learning. In the area of multi-robot collaboration, I contributed to the development of a relative localization system, CREPES (with a related article submitted to IEEE TRO). In mechanical design, I participated in the development of a reconfigurable tracked robot, CubeTrack (with a related paper accepted as an oral presentation at IROS 2024). Previously, I served as a reviewer for ICRA and IROS conferences. -->
<!-- - **Multi-Robot Perception:** continuous-time SLAM, multi-robot SLAM, relative state estimation, distributed algorithm

- **Mechanical design:** innovation structures, tracked robots, kinematics and dynamics analysis -->

My research focuses on robotic perception, including ego-state estimation for individual robots and collaborative perception for multi-robot systems. I am particularly interested in developing accurate and real-time state estimation algorithms that enable robots to perceive themselves, localize their teammates, and operate robustly in complex real-world environments.

<!-- - **Continuous-Time State Estimation:** real-time continuous-time SLAM, LiDAR-visual-inertial SLAM
- **Multi-Robot Systems:** relative state estimation, distributed optimization, air-ground cooperation -->

## News
- **[Feb. 2026]** Our paper about continuous-time multi-robot direct relative localization is submitted to IEEE TRO.
- **[Dec. 2025]** Our paper about multi-robot direct relative localization is submitted to IEEE TRO.
- **[Oct. 2025]** Our demonstration about air-ground cooperation is accpeted by IROS 2025 EXPO.
- **[Jul. 2025]** Our paper about learning-based relative localization is accpeted by IROS 2025.
- **[Jul. 2024]** Our paper about reconfigurable tracked robot is accepted by IROS 2024.

{% include_relative _includes/ongoings.md %}

{% include_relative _includes/publications.md %}

{% include_relative _includes/projects.md %}

{% include_relative _includes/services.md %}
