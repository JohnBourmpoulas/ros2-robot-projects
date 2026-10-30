# ROS 2 Robot Projects

A collection of robotics projects focused on robot modeling, simulation, and software development using ROS 2.

This repository documents my practical experience with robotics technologies, starting with basic robot descriptions and gradually progressing toward more complex robotic systems.

The long-term objective is to develop the skills required to design, simulate, program, and build robotic systems.

## Overview

Each project is organized in a separate directory and includes its source files, documentation, and relevant visualization results.

The repository covers topics such as:

- Robot modeling using URDF
- Coordinate frames and transformations using TF2
- Robot visualization with RViz2
- Physics-based simulation with Gazebo
- Robot control and ROS 2 development
- Mechanical design and CAD integration

## Technologies

| Technology | Purpose |
|---|---|
| ROS 2 Jazzy | Robotics middleware and software development |
| URDF | Robot structure and kinematic descriptions |
| RViz2 | Robot visualization and debugging |
| TF2 | Coordinate transformations |
| Gazebo | Physics-based robot simulation |
| Python / C++ | ROS 2 application development |
| FreeCAD | Mechanical design and 3D modeling |

Some technologies listed above are planned for future projects.

## Projects

| Project | Description | Status |
|---|---|---|
| [01 - First URDF Robot](01-first-robot/) | Basic mobile robot model with a rectangular chassis and two wheels | In Progress |

Additional projects will be added as development progresses.

## Repository Structure

```text
ros2-robot-projects/
├── README.md
├── LICENSE
├── .gitignore
│
├── 01-first-robot/
│   ├── README.md
│   ├── my_robot.urdf
│   └── images/
│
└── ...
```

## Development Approach

Projects in this repository follow an incremental development process:

1. Define the robot's structure and components.
2. Create the robot description using URDF.
3. Visualize and validate the model in RViz2.
4. Integrate the model into Gazebo for simulation.
5. Implement robot control and ROS 2 functionality.
6. Explore mechanical design and physical implementation.

Not every project includes all development stages.

## Project Goals

The primary goals of this repository are to:

- Develop practical knowledge of ROS 2 and its ecosystem.
- Understand robot coordinate systems, links, and joints.
- Gain experience with robot modeling and simulation.
- Improve robotics programming and debugging skills.
- Explore the integration of software and mechanical design.
- Build a documented portfolio of robotics projects.

## License

This project is licensed under the [MIT License](LICENSE).
