3-DOF Robotic Arm

A simple 3-Degree-of-Freedom (3-DOF) robotic arm developed using URDF and visualized in RViz2 with ROS 2 Jazzy.

The robot features a rotating base, a shoulder joint, and an elbow joint, allowing movement across three rotational axes.

This project demonstrates fundamental concepts of robot modeling, including links, joints, coordinate frames, and joint limits.

⸻

Robot Preview

3-DOF robotic arm visualized in RViz2.

⸻

Features

* 3 Degrees of Freedom (3-DOF)
* Base rotation: −90° to +90° (180° total range)
* Shoulder rotation: −90° to +90°
* Elbow rotation: −135° to +135°
* URDF model using basic geometric shapes
* Revolute joints with defined rotation limits
* Interactive joint control using Joint State Publisher GUI
* Robot visualization in RViz2

⸻

Robot Structure

The robotic arm consists of the following components:

Component	Description
base_footprint	Ground reference frame
base_link	Fixed base
rotating_base_link	Rotating platform
upper_arm_link	Upper arm (30 cm)
forearm_link	Forearm (25 cm)
tool_link	End-effector placeholder

Joint Configuration

Joint	Type	Axis	Range
base_rotation_joint	Revolute	Z	−90° to +90°
shoulder_joint	Revolute	Y	−90° to +90°
elbow_joint	Revolute	Y	−135° to +135°

⸻

Requirements

* ROS 2 Jazzy
* RViz2
* urdf_tutorial
* joint_state_publisher_gui

⸻

Running in RViz2

Launch the robot model using:

ros2 launch urdf_tutorial display.launch.py model:=/path/to/my_robotic_arm.urdf

Replace /path/to/my_robotic_arm.urdf with the actual path to the URDF file.

Use the Joint State Publisher GUI to control the three revolute joints interactively.

⸻

Project Structure

02-3dof-robotic-arm/
├── my_robotic_arm.urdf
├── README.md
└── images/
    └── robotic_arm_rviz.png

⸻

Notes

This project focuses on URDF modeling and robot visualization in RViz2.

The current model does not include collision geometry, inertial properties, or simulation controllers for physics-based simulation in Gazebo.
