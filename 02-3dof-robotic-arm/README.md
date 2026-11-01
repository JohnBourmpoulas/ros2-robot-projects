# 3-DOF Robotic Arm

A 3-degree-of-freedom robotic arm modeled in URDF and visualized using ROS 2 Jazzy and RViz2.

<p align="center">
  <img src="./images/robotic_arm_rviz.png" alt="3-DOF Robotic Arm in RViz2" width="750">
</p>

<p align="center">
  <em>3-DOF robotic arm visualization in RViz2</em>
</p>

## Overview

This project demonstrates the fundamentals of robot modeling using the Unified Robot Description Format (URDF).

The robotic arm consists of a fixed base, a rotating platform, two articulated arm segments, and an end-effector placeholder.

The model includes three revolute joints with defined motion limits, allowing interactive visualization and joint manipulation in RViz2.

## Joint Configuration

| Joint | Rotation Axis | Motion Range |
|:------|:-------------:|:------------:|
| Base | Z | −90° to +90° |
| Shoulder | Y | −90° to +90° |
| Elbow | Y | −135° to +135° |

## Technical Specifications

| Parameter | Value |
|:----------|:------|
| Degrees of Freedom | 3 |
| Robot Description | URDF |
| ROS Distribution | ROS 2 Jazzy |
| Visualization | RViz2 |
| Upper Arm Length | 0.30 m |
| Forearm Length | 0.25 m |
| Joint Types | Revolute, Fixed |

## Requirements

- ROS 2 Jazzy
- RViz2
- `urdf_tutorial`
- `joint_state_publisher_gui`

## Visualization

Launch the robot model in RViz2:

```bash
ros2 launch urdf_tutorial display.launch.py model:=/path/to/my_robotic_arm.urdf
```

Replace `/path/to/my_robotic_arm.urdf` with the actual location of the URDF file.

The Joint State Publisher GUI provides interactive sliders for controlling the base, shoulder, and elbow joints within their defined limits.

## Project Structure

```text
02-3dof-robotic-arm/
├── images/
│   └── robotic_arm_rviz.png
├── my_robotic_arm.urdf
└── README.md
```

## Current Scope

The project focuses on robot description, kinematic structure, and visualization.

Physics-based simulation in Gazebo is not currently implemented. Collision geometry, inertial properties, and simulation controllers would be required for further development.
