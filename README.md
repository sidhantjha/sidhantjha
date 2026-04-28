<div align="center">

<img src="https://raw.githubusercontent.com/sidhantjha/sidhantjha/main/banner.svg" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=15&duration=3000&pause=1200&color=38BDF8&center=true&vCenter=true&width=700&lines=Building+robots+that+think+for+themselves.;Perception+%C2%B7+Control+%C2%B7+Decentralized+Intelligence;Aerospace+Engineering+%2B+CS+%40+UIUC" alt="Typing SVG" />

[![LinkedIn](https://img.shields.io/badge/-LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/sidhantsjha)
&nbsp;
[![Email](https://img.shields.io/badge/-SSJHA2@ILLINOIS.EDU-38BDF8?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ssjha2@illinois.edu)
&nbsp;
[![UIUC](https://img.shields.io/badge/-AEROSPACE_@_UIUC-13294B?style=for-the-badge&logo=academia&logoColor=white)](https://aerospace.illinois.edu)
&nbsp;
[![YouTube](https://img.shields.io/badge/-VOS_STUDIOS-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtube.com)

</div>

---

<div align="center">
<br/>

**Autonomy-focused engineer at the intersection of perception, control theory, and decentralized multi-robot coordination.**

<br/>

`ACRL` &nbsp;·&nbsp; `AVIATE` &nbsp;·&nbsp; `MIT SPARK Lab` &nbsp;·&nbsp; `Project Lumyn` &nbsp;·&nbsp; `rosscope`

<br/>
</div>

---

## Research

| Lab | Role | Focus Area |
|-----|------|------------|
| **[ACRL](https://naira.mechse.illinois.edu/)**, UIUC | Undergraduate Researcher | ROS 2 + Hydra 3D Scene Graph mapping; joint NSF CPS project with MIT SPARK Lab (Prof. Luca Carlone, MIT AeroAstro) under Prof. Naira Hovakimyan |
| **[AVIATE](https://aviate.aerospace.illinois.edu/)**, UIUC | Student Researcher | Shared human–AI autonomy via game-theoretic Nash equilibrium switching; extending Flip_Alt framework to UAVs and multi-robot systems |
| **IAMPL** *(Rolls-Royce × HAL JV)* | Engineering Intern | Parametric aerospace component design in Siemens NX under GD&T constraints for Trent 1000 program |

---

## Projects

### [`hydra_tb4_autonomy`](https://github.com/sidhantjha/hydra_tb4_autonomy) — ROS 2 + Hydra 3D Scene Graph Stack
> 3D Scene Graphs · TSDF Reconstruction · LLM-based Semantic Planning · Nav2

Deployed MIT SPARK Lab's Hydra Dynamic Scene Graph pipeline on ROS 2 Jazzy as the world representation layer in a joint NSF CPS perception-planning-control architecture (UIUC × MIT). Engineered a full sensor integration pipeline bridging TurtleBot3 Gazebo to Hydra's uHumans2 format — remapping 8 sensor topics, resolving TF inconsistencies across 5+ coordinate frames, modifying the TurtleBot3 Waffle SDF model to add 32FC1 depth sensing, and extending TSDF max_range from 5m to 10m for 60% improved depth coverage. Traced and resolved a silent Gazebo sensor bridge misconfiguration causing TSDF integration failure despite all pipeline components appearing active.

`ROS 2` `Hydra` `Nav2` `Gazebo` `TSDF` `C++` `Python`

---
### [`drone-gate-perception`](https://github.com/sidhantjha/skysync_anduril_grand_prix.git)) — Gate Perception and Pose Estimation for Autonomous Drone Racing
> CNN · U-Net · Keypoint Detection · YOLO-Pose · PnP · Kalman Filter · TII Dataset

Comparative computer vision pipeline evaluating four perception front-ends — CNN classification, U-Net segmentation, custom heatmap keypoint CNN, and YOLO-Pose — for racing-gate detection and corner localization on the TII Race Against the Machine dataset. Connects best-performing perception outputs to PnP pose estimation (solvePnP) and Kalman filter state estimation, evaluated against mocap ground truth. Metrics span classification accuracy, mask IoU, corner error, PCK, PnP reprojection error, and downstream state-estimation RMSE.

`Python` `PyTorch` `OpenCV` `YOLO-Pose` `PnP` `Kalman Filter`

---

### [`AVIATE-SharedAutonomy`](https://github.com/sidhantjha/aviate-shared-autonomy) — Human–AI Cooperative Control
> Game Theory · Nash Equilibrium Switching · Stochastic Override Models

Investigating shared autonomy between human and AI agents for general dynamical systems using game-theoretic formulations. Implementing cooperative takeover policies from identical-interest dynamic games and Nash equilibrium switching strategies. Analyzing cost-sensitive authority transitions via linear–quadratic saddle-point recursions under stochastic human override models (pₖ). Benchmarking against ad-hoc baselines in OpenAI Gymnasium under disturbance and partial observability. Extending the Flip_Alt framework beyond self-driving to UAV and multi-robot domains.

`Python` `OpenAI Gymnasium` `Control Theory` `Game Theory` `LQR` `PyTorch`

---

### [`SkySync`](https://github.com/sidhantjha/SkySync_Hybrid_Multi_UAV_Swarm_Controller.git) — Decentralized Multi-UAV Formation Control
> APF · Consensus ADMM · MPC · Peer-Reviewed · Anduril AI Grand Prix

Designed and validated a hybrid control architecture combining Artificial Potential Fields, Consensus ADMM, and Model Predictive Control for simultaneous UAV swarm formation maintenance and obstacle avoidance. **Published and presented** at the AIAA Region III Student Conference, University of Michigan. Validated across 80 simulation trials: 80% mission success rate, 70.4% collision reduction vs. standalone APF, zero obstacle penetrations across all 20 hybrid trials. Hardware deployment on Crazyflie 2.1+. **Currently competing in the Anduril AI Grand Prix Drone Swarm Competition.**

`ROS 2` `Python` `C++` `Webots` `Crazyflie` `Control Theory` `Multi-Agent Systems`

---

### [`AutoDock`](https://github.com/sidhantjha/autodock) — Autonomous Racing @ ICRA 2026
> F1TENTH · SLAM · MPCC · Pure Pursuit · Rob Racer Sim Racing League

**Competing in the Rob Racer Sim Racing League at ICRA 2026** (F1TENTH platform). Building and benchmarking a full algorithm stack: minimum-curvature racing line optimization, Pure Pursuit tracking, Model Predictive Contouring Control (MPCC), Model and Acceleration-based Pursuit (MAP) with Pacejka tire dynamics, and minimum-time trajectory optimization via CasADi + IPOPT. Unknown-track pipeline: SLAM (slam_toolbox) → racing line extraction → particle filter localization → Pure Pursuit, with Follow-the-Gap and Disparity Extender as reactive fallbacks. Hybrid mode-switching state machine for qualification and time-attack rounds.

`ROS 2` `Python` `C++` `SLAM` `MPC` `CasADi` `F1TENTH`

---

### [`AirframeX`](https://github.com/sidhantjha/airframex) — Low-Level Quadrotor Flight Control
> PID · Reinforcement Learning · Euler–Lagrange Dynamics · PX4

Implementing and tuning PID controllers on Pixhawk-based quadrotors for roll, pitch, and thrust stabilization. Engineering RL state-machine policies to optimize motor thrust under nonlinear flight dynamics. Modeling propeller-arm torque–thrust coupling via Euler–Lagrange formulation. Configured PX4 flight control systems including motor mapping, ESC calibration, PWM/OneShot/DShot protocols, and RC input via QGroundControl and MAVLink.

`C++` `Python` `Pixhawk` `PX4` `ROS 2` `MAVSDK`

---

## Stack

**Robotics & Middleware**

![ROS2](https://img.shields.io/badge/ROS_2-22314E?style=flat-square&logo=ros&logoColor=white)
![Gazebo](https://img.shields.io/badge/Gazebo-FF6600?style=flat-square&logo=gazebo&logoColor=white)
![Nav2](https://img.shields.io/badge/Nav2-222222?style=flat-square&logo=ros&logoColor=white)
![Isaac Sim](https://img.shields.io/badge/Isaac_Sim-76B900?style=flat-square&logo=nvidia&logoColor=white)
![Webots](https://img.shields.io/badge/Webots-1E293B?style=flat-square&logoColor=white)

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=flat-square&logo=mathworks&logoColor=white)

**Perception & Mapping**

![Visual SLAM](https://img.shields.io/badge/Visual_SLAM-1E293B?style=flat-square&logoColor=white)
![Hydra](https://img.shields.io/badge/Hydra_(MIT_SPARK)-1E293B?style=flat-square&logoColor=white)
![Kimera](https://img.shields.io/badge/Kimera_VIO-1E293B?style=flat-square&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)

**Control & Decision-Making**

![MPC](https://img.shields.io/badge/MPC-0F172A?style=flat-square&color=0F172A)
![LQR](https://img.shields.io/badge/LQR-0F172A?style=flat-square)
![L1 Adaptive](https://img.shields.io/badge/L1_Adaptive_Control-0F172A?style=flat-square)
![Game Theory](https://img.shields.io/badge/Game--Theoretic_Switching-0F172A?style=flat-square)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Gymnasium](https://img.shields.io/badge/OpenAI_Gymnasium-0081A5?style=flat-square)

**UAV & Hardware**

![PX4](https://img.shields.io/badge/PX4-5C3EE8?style=flat-square&logoColor=white)
![MAVSDK](https://img.shields.io/badge/MAVSDK-1E293B?style=flat-square&logoColor=white)
![Crazyflie](https://img.shields.io/badge/Crazyflie_2.1+-1E293B?style=flat-square&logoColor=white)
![Pixhawk](https://img.shields.io/badge/Pixhawk-1E293B?style=flat-square&logoColor=white)

**Design & Tools**

![Siemens NX](https://img.shields.io/badge/Siemens_NX-009999?style=flat-square)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

---

## Currently Building

```
[■■■■■■■□□□]  rosscope              — AI debugging layer for ROS 2 (startup)
[■■■■■■■■■□]  SkySync               — Competing: Anduril AI Grand Prix Drone Swarm Competition
[■■■■■■□□□□]  AutoDock              — Competing: Rob Racer Sim Racing League @ ICRA 2026
[■■■■■■■■□□]  AVIATE Research       — Game-theoretic shared autonomy benchmarks
[■■■■■■■■■□]  ACRL / MIT SPARK      — Hydra 3D Scene Graph + certifiable UAV control (NSF CPS)
[■■■■■□□□□□]  AirframeX             — RL + PID on Pixhawk quadrotor
```

---

## Project Lumyn

[**Project Lumyn**](https://github.com/project-lumyn) is a robotics autonomy organization I founded at UIUC's AIAA chapter, leading 20+ engineers across perception, control, and multi-agent systems research.

| Initiative | Status | Description |
|------------|--------|-------------|
| **SkySync** | ✅ Conference Paper Published · 🏆 Anduril AI Grand Prix | Hybrid APF + Consensus ADMM + MPC swarm control — presented at AIAA Region III, University of Michigan |
| **AutoDock** | 🏁 ICRA 2026 Competitor | Autonomous racing on F1TENTH platform — SLAM + MPCC + Pure Pursuit pipeline |
| **EchoNav** | 🔨 Active Development | Sensor-based obstacle-aware navigation stack with LiDAR + OpenCV |

---

## Publications

**"Toward Real-World Swarm Deployment: A Hybrid APF–ADMM–MPC Control Architecture for Path Planning in Multi-UAV Systems"**
Yuvraj Agarwal, Sidhant Jha, Neil Kashid, Robbie Harris, Aditya Choksi
*AIAA Region III Student Conference, University of Michigan, 2025*

---

<div align="center">

*"The goal is not to build a robot. The goal is to build a robot that can figure out what to do next."*

<br/>

[![GitHub Streak](https://streak-stats.demolab.com?user=sidhantjha&theme=tokyonight-duo&hide_border=true&background=0D1117&stroke=38BDF8&ring=38BDF8&fire=38BDF8&currStreakLabel=38BDF8&sideLabels=94A3B8&dates=94A3B8&currStreakNum=F0F9FF&sideNums=F0F9FF)](https://github.com/sidhantjha)

</div>
