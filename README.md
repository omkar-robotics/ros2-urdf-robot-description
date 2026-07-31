# ROS 2 URDF Robot Description

This project demonstrates how to create and visualize a simple mobile robot using URDF in ROS 2 Humble.

## Features

- Robot modeled using URDF
- Differential drive robot structure
- Base link and base footprint
- Two continuous wheel joints
- Fixed caster wheel
- LiDAR sensor model
- Launch file for visualization
- Robot visualization in RViz2
- Robot State Publisher
- Joint State Publisher GUI

## Project Structure

```
my_urdf/
├── src/
│   └── my_pkg/
│       ├── launch/
│       │   └── display.launch.py
│       ├── urdf/
│       │   └── my_robot.urdf
│       ├── CMakeLists.txt
│       └── package.xml
```

## Requirements

- Ubuntu 22.04
- ROS 2 Humble

## Build

```bash
cd ~/my_urdf
colcon build
source install/setup.bash
```

## Run

```bash
ros2 launch my_pkg display.launch.py
```

## Learning Outcomes

- Creating links in URDF
- Creating joints in URDF
- Using materials and colors
- Robot State Publisher
- Joint State Publisher GUI
- RViz2 visualization
- ROS 2 package structure