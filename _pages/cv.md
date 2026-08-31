---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Bo-Rong (Philip) Lai — Robotics Software Engineer
[philipt710mh@gmail.com](mailto:philipt710mh@gmail.com) · +886 920 510 265 · [LinkedIn](https://www.linkedin.com/in/bo-rong-lai-24765320b/) · [GitHub](https://github.com/UrMBCMRabbont)

Education
======
* **BEng in Electronic and Computer Engineering, Minor in Robotics**, The Hong Kong University of Science and Technology, Hong Kong S.A.R., China, Sep 2020 – Jun 2024

Work experience
======
* **Mar 2026 – Aug 2026: Robotics Software Engineer**, Dimeidos, Kaohsiung, Taiwan
  * Enhanced posture alignment in **7-DOF teleoperation** by constraining the robot arm using the operator's elbow angle, with a simulated **Pareto analysis** proving superior end-effector accuracy over an elbow-position multi-node IK formulation.
  * Designed a joint-calibration workflow that reduced reconstruction error to **11%**, enabling real-time swivel angle extraction from **RealSense D435i** pose estimates (GPU-accelerated VINS-Fusion) to drive a PyBullet IK solver on the OpenArm.
  * Extended **ACT** for bimanual imitation learning: swapped its ResNet-18 vision encoder for a DINO backbone, raising task success rate by **20%** on a cube-grasping task with an **SO-101** arm, and refactored temporal ensembling to expose configurable action-chunk size and inference stride for controlled ablation.

* **Nov 2024 – Feb 2026: Robotics Software Engineer**, Aiseed Technology, Taipei, Taiwan
  * Deployed **OpenVINS** visual-inertial odometry on a 4 GB Jetson Nano alongside a PX4 flight controller, sustaining **250 m** of autonomous flight at **80 m** altitude in **GNSS-denied environments**.
  * Collaborated with the ESC hardware department to bring up and validate an in-house **ESC** design running **AM32** motor-control firmware during the prototyping phase.

* **Jun 2023 – Aug 2023: Summer Intern**, Skyland Innovation, HKCRC, Dongguan, China
  * Built a LiDAR-based autonomous navigation system on a bipedal robot in **ROS 2**, integrating an open-source online mapping module into the existing **SLAM** stack.

* **Jun 2022 – Aug 2022: Summer Research Intern**, Academia Sinica, Taipei, Taiwan
  * Added power-loss recovery to an existing BLE telemetry stack on STM32 Nucleo-WB (**FreeRTOS**): on low-voltage detection, checkpointed the last transmitted packet to non-volatile memory over **SPI**, so transmission resumed from the checkpoint instead of restarting.

Academic projects
======
* **Mobile Robot Navigation & State Estimation** — HKUST Course Project, Hong Kong, Sep 2023 – Dec 2023
  * Mapping & localization: implemented **ICP** point-cloud registration to improve odometry accuracy, and an **EKF** for multi-landmark data association on a point-cloud map.

* **HKUST Robotics Team** — Team Member, Embedded Software Dept., Hong Kong, Nov 2021 – Jun 2022
  * Built a 4-wheeled independent-steering competition robot on an **STM32** F4 platform with a **FreeRTOS** multi-task architecture, and implemented its **PD**-based autonomous driving system.
  * Achieved the fastest completion time, **1st Runner-Up** and **Best Engineering Award** among **14** university teams at the 2022 Hong Kong **ABU** Robocon Contest.

Skills
======
* **Languages**: C++, C, Python, Bash
* **Robotics & middleware**: ROS 2 (ros2_control, Nav2, DDS/CycloneDDS), ROS, PX4, PyBullet, MuJoCo, Gazebo
* **Perception & state estimation**: VIO, EKF, ICP, FAST-LIO2, ORB-SLAM3
* **Robot learning**: PyTorch, LeRobot, imitation learning (ACT, Diffusion Policy), VLA (Pi0.5)
* **Embedded & systems**: STM32, FreeRTOS, motor control / ESC, BLE, Linux, Docker, Git

Awards
======
* **1st Runner-Up** and **Best Engineering Award**, 2022 Hong Kong ABU Robocon Contest
