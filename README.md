# 🤖 ROS 2 URDF Mobile Robot Description

![ROS2](https://img.shields.io/badge/ROS2-Humble-blue)
![URDF](https://img.shields.io/badge/Robot-URDF-green)
![RViz2](https://img.shields.io/badge/Visualization-RViz2-orange)
![Robot State Publisher](https://img.shields.io/badge/Node-Robot_State_Publisher-red)
![License](https://img.shields.io/badge/License-Apache--2.0-yellow)

🚀 **A ROS 2 Humble project demonstrating how to build and visualize a differential drive mobile robot using URDF, Robot State Publisher, Joint State Publisher GUI, and RViz2.**

This project focuses on creating a robot model from scratch using **URDF (Unified Robot Description Format)** and visualizing it in **RViz2**. It serves as a foundational project for learning robot modeling before moving on to Gazebo simulation, ROS2 Control, SLAM, and Navigation2.

---

# 📌 Project Overview

This project demonstrates how to design a simple differential drive robot in ROS 2 using URDF.

The robot consists of:

* A rectangular robot base
* Two continuous drive wheels
* One caster wheel
* A LiDAR sensor mounted on top

The robot model is published using **Robot State Publisher**, its joints are controlled using **Joint State Publisher GUI**, and the complete robot is visualized in **RViz2**.

---

# 🔑 Key Concepts Demonstrated

* Robot modeling using URDF
* ROS 2 package structure
* Links and Joints
* Fixed and Continuous joints
* Robot coordinate frames
* Robot visualization using RViz2
* Robot State Publisher
* Joint State Publisher GUI

---

# 🛠️ Technologies Used

| Technology                        | Description                |
| --------------------------------- | -------------------------- |
| 🤖 **ROS 2 Humble**               | Robotics middleware        |
| 📄 **URDF**                       | Robot description format   |
| 🎯 **RViz2**                      | Robot visualization        |
| 🔄 **Robot State Publisher**      | Publishes robot transforms |
| 🎛️ **Joint State Publisher GUI** | Controls movable joints    |
| ⚙️ **CMake**                      | ROS 2 build system         |
| 🐧 **Ubuntu 22.04**               | Operating System           |

---

# ⚙️ System Workflow

The project workflow follows these steps:

1️⃣ Build the ROS 2 workspace

2️⃣ Source the workspace

3️⃣ Launch the robot visualization

4️⃣ Robot State Publisher publishes the TF tree

5️⃣ Joint State Publisher GUI updates wheel joint states

6️⃣ RViz2 displays the complete robot model

---

# 💻 System Requirements

Before running this project, ensure the following software is installed:

* Ubuntu 22.04
* ROS 2 Humble
* RViz2
* Robot State Publisher
* Joint State Publisher GUI
* Colcon Build System

---

# 📂 Project Structure

```text
my_urdf/
│
├── README.md
├── images/
│   ├── robot_model.png
│   ├── joint_state_publisher.png
│   └── rviz_visualization.png
│
└── src/
    └── my_pkg/
        ├── launch/
        │   └── display.launch.py
        ├── urdf/
        │   └── my_robot.urdf
        ├── CMakeLists.txt
        └── package.xml
```

---

# 🖥️ Project Demonstration

---

## 1️⃣ Robot Description

The robot model is created entirely using **URDF**.

### 📷 Robot Model

<img width="100%" src="Screenshot from 2026-07-31 16-12-27.png"/>

The robot includes:

* Base Link
* Base Footprint
* Left Wheel
* Right Wheel
* Caster Wheel
* LiDAR Sensor

---

## 2️⃣ Joint State Publisher GUI

The Joint State Publisher GUI allows interactive movement of continuous joints for visualization.

<img width="100%" src="images/joint_state_publisher.png"/>

### ▶️ Launch Command

```bash
ros2 launch my_pkg display.launch.py
```

This starts:

* Robot State Publisher
* Joint State Publisher GUI
* RViz2

---

## 3️⃣ RViz2 Visualization

The robot is visualized in RViz2 using TF frames published by Robot State Publisher.

<img width="100%" src="images/rviz_visualization.png"/>

The visualization helps verify:

* Robot geometry
* Link hierarchy
* Joint configuration
* Robot transforms (TF)

---

# ▶️ Build the Project

```bash
cd ~/my_urdf

colcon build

source install/setup.bash
```

---

# ▶️ Run the Project

```bash
ros2 launch my_pkg display.launch.py
```

---

# ✨ Features

✅ Robot modeled entirely using URDF

✅ Differential drive robot structure

✅ Base Link and Base Footprint

✅ Continuous wheel joints

✅ Fixed caster wheel

✅ LiDAR sensor model

✅ Robot State Publisher integration

✅ Joint State Publisher GUI

✅ RViz2 visualization

✅ Clean ROS 2 package organization

---

# 📚 Learning Outcomes

Through this project, I learned:

* Creating robot models using URDF
* Understanding robot links and joints
* Working with Fixed and Continuous joints
* Defining materials and colors
* Building ROS 2 packages
* Installing package resources
* Using Robot State Publisher
* Using Joint State Publisher GUI
* Visualizing robots in RViz2
* Understanding the TF frame hierarchy

---

# 🚀 Future Improvements

Planned enhancements include:

* Add collision geometry
* Add inertial properties
* Convert URDF to Xacro
* Integrate Gazebo simulation
* Add LiDAR plugins
* Add camera sensor
* Integrate ROS2 Control
* Prepare robot for SLAM
* Navigation2 integration

---

# 👨‍💻 Author

**Omkar Maroti Honrao**

**B.Tech Electrical Engineering Student**

**Robotics Research Intern**

**Skills:** ROS 2 • Python • URDF • Gazebo • RViz2 • OpenCV • Navigation2 • SLAM

GitHub: https://github.com/omkar-robotics

---

# ⭐ Support

If you found this project helpful, consider giving it a **⭐ Star** on GitHub.

Your support motivates me to continue building and sharing more ROS 2 and Robotics projects.
