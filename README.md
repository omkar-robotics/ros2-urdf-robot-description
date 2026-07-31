# 🤖 ROS 2 URDF Mobile Robot Description

A beginner-friendly ROS 2 Humble project demonstrating how to design, structure, and visualize a simple differential drive mobile robot using **URDF (Unified Robot Description Format)** and **RViz2**.

This project focuses on building the robot model from scratch, defining links and joints, and visualizing the robot using ROS 2 visualization tools.

---

## 📌 Overview

This project creates a simple mobile robot consisting of:

* Rectangular robot base
* Two continuous drive wheels
* One caster wheel
* LiDAR sensor mounted on top
* Robot visualization in RViz2
* Robot State Publisher
* Joint State Publisher GUI

The project provides a solid foundation for learning robot modeling before moving on to Gazebo simulation, SLAM, Navigation2 (Nav2), and autonomous robotics.

---

## 🚀 Features

* ✅ Robot modeled completely in URDF
* ✅ Differential drive robot structure
* ✅ Base Footprint and Base Link
* ✅ Continuous wheel joints
* ✅ Fixed caster wheel
* ✅ LiDAR sensor representation
* ✅ Robot State Publisher integration
* ✅ Joint State Publisher GUI
* ✅ RViz2 visualization
* ✅ ROS 2 package structure using CMake

---

## 🛠️ Technologies Used

* ROS 2 Humble
* URDF
* RViz2
* Robot State Publisher
* Joint State Publisher GUI
* CMake
* Ubuntu 22.04

---

## 📁 Project Structure

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

## ⚙️ Prerequisites

Before running this project, make sure you have:

* Ubuntu 22.04
* ROS 2 Humble
* RViz2
* Robot State Publisher
* Joint State Publisher GUI
* Colcon Build System

---

## 📦 Build the Project

```bash
cd ~/my_urdf

colcon build

source install/setup.bash
```

---

## ▶️ Run the Project

Launch the robot visualization:

```bash
ros2 launch my_pkg display.launch.py
```

This launch file starts:

* Robot State Publisher
* Joint State Publisher GUI
* RViz2

---

# 📷 Output

## Robot Visualization

> Replace the image paths below after uploading your screenshots.

### Robot Model

![Robot Model](images/Screenshot%20from%202026-07-31%2016-12-27.png)

---

### Joint State Publisher

![Joint State Publisher](images/Screenshot%20from%202026-07-31%2016-12-34.png)

---

### RViz2 Visualization

![RViz2](images/Screenshot%20from%202026-07-31%2016-12-43.png)

---

## 📚 Learning Outcomes

Through this project, I learned:

* Creating robot models using URDF
* Understanding Links and Joints
* Using Fixed and Continuous joints
* Defining robot materials and colors
* Organizing a ROS 2 package
* Launching multiple ROS 2 nodes
* Visualizing robots in RViz2
* Working with Robot State Publisher
* Using Joint State Publisher GUI

---

## 🔮 Future Improvements

Planned enhancements include:

* Add Xacro support
* Add robot inertial properties
* Add collision models
* Integrate Gazebo simulation
* Add LiDAR plugin
* Add camera sensor
* Implement ROS 2 Control
* Perform SLAM using slam_toolbox
* Autonomous Navigation using Nav2

---

## 👨‍💻 Author

**Omkar Honrao**

B.Tech Electrical Engineering Student

Robotics | ROS 2 | Python | Gazebo | RViz2 | OpenCV | Navigation2 | SLAM

GitHub: https://github.com/omkar-robotics

---

## ⭐ Support

If you found this project helpful, consider giving it a **⭐ Star** on GitHub.

It motivates me to continue building and sharing more ROS 2 and Robotics projects.
