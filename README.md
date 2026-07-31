# ROS 2 URDF Robot Description

A beginner-friendly ROS 2 Humble project that demonstrates how to design, organize, and visualize a mobile robot using the Unified Robot Description Format (URDF). The robot can be visualized in RViz2 using **Robot State Publisher** and **Joint State Publisher GUI**, making it an excellent starting point for learning robot modeling in ROS 2.

---

## Overview

This project creates a simple differential-drive mobile robot with:

* A rectangular base
* Two continuous drive wheels
* One caster wheel
* A LiDAR sensor mounted on top
* URDF-based robot description
* RViz2 visualization
* Interactive joint control using Joint State Publisher GUI

The project focuses on understanding the fundamentals of robot modeling before moving to simulation platforms such as Gazebo.

---

## Robot Structure

The robot consists of the following components:

| Component      | Description                     |
| -------------- | ------------------------------- |
| Base Footprint | Root frame of the robot         |
| Base Link      | Main body of the robot          |
| Left Wheel     | Continuous rotating wheel       |
| Right Wheel    | Continuous rotating wheel       |
| Caster Wheel   | Fixed support wheel             |
| LiDAR Sensor   | Simple cylindrical sensor model |

---

## Project Structure

```text
my_urdf/
├── src/
│   └── my_pkg/
│       ├── launch/
│       │   └── display.launch.py
│       ├── urdf/
│       │   └── my_robot.urdf
│       ├── CMakeLists.txt
│       └── package.xml
├── README.md
└── .gitignore
```

---

## Prerequisites

* Ubuntu 22.04
* ROS 2 Humble
* colcon
* RViz2
* Robot State Publisher
* Joint State Publisher GUI

---

## Build Instructions

Clone the repository:

```bash
git clone https://github.com/omkar-robotics/ros2-urdf-robot-description.git
```

Move into the workspace:

```bash
cd ros2-urdf-robot-description
```

Build the package:

```bash
colcon build
```

Source the workspace:

```bash
source install/setup.bash
```

---

## Launch the Robot

Run the launch file:

```bash
ros2 launch my_pkg display.launch.py
```

This starts:

* Robot State Publisher
* Joint State Publisher GUI
* RViz2

---

## Features

* Clean ROS 2 package structure
* Robot modeled using URDF
* Fixed and continuous joints
* Multiple robot links
* Custom materials and colors
* Differential-drive robot layout
* LiDAR sensor representation
* RViz2 visualization
* Robot State Publisher integration
* Joint State Publisher GUI support

---

## Technologies Used

* ROS 2 Humble
* URDF
* RViz2
* Robot State Publisher
* Joint State Publisher GUI
* CMake
* XML

---

## Learning Outcomes

After completing this project, you will understand:

* ROS 2 package organization
* URDF syntax and structure
* Creating robot links
* Creating fixed and continuous joints
* Defining materials and colors
* Robot coordinate frames
* Robot visualization in RViz2
* Robot State Publisher workflow
* Joint State Publisher GUI usage
* Preparing a robot model for future Gazebo simulation

---

## Future Improvements

Planned enhancements include:

* Add collision geometry
* Add inertial properties
* Convert URDF to Xacro
* Integrate Gazebo simulation
* Add differential drive plugin
* Add LiDAR simulation
* Integrate SLAM Toolbox
* Integrate Navigation2 (Nav2)

---

## Author

**Omkar Honrao**

B.Tech Electrical Engineering Student

Robotics & ROS 2 Enthusiast

GitHub: https://github.com/omkar-robotics

---

## License

This project is licensed under the Apache 2.0 License.

---

## Acknowledgements

This project was developed as part of my ROS 2 learning journey to build a strong foundation in robot modeling, visualization, and autonomous robotics development.
