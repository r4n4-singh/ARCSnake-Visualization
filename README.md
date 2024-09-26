# ARCSnake Voodoo Doll Visualizer

## Overview
This ROS2 package provides the necessary configuration to simulate a snake-like robot using URDF in RViz. It includes a detailed URDF model with multiple configurable joints and visual properties, which can be visualized and interacted with in real-time through RViz.

## How to Set Up

### Prerequisites
Ensure you have a ROS2 environment set up (e.g., Foxy, Humble) with RViz installed. 

### Building the Package
Navigate to your ROS2 workspace and clone this repository into the `src` directory. Then, build the package using `colcon`:

```bash
cd ~/dev_ws  # Adjust path as needed
colcon build --packages-select snake_robot
source install/setup.bash
```

## How to Use
To launch the simulation:

```bash
ros2 launch snake_robot snake_robot.launch.py
```

This command initializes the ROS environment, loads the URDF configuration, and sets up RViz for real-time visualization of the snake robot's movement.

## Directory Structure
Here is an outline of the key directories and files within this package:

- `config/`: Configuration files.
- `launch/`: ROS2 launch files.
- `meshes/`: Mesh files for the robot model.
- `models/`: Model files.
- `params/`: Parameter files.
- `rviz/`: RViz configuration files.
- `urdf/`: URDF files describing the robot structure.

## Needed Libraries
Ensure you have the following ROS2 packages installed:

- `rclpy`
- `rviz2`
- `robot_state_publisher`
- `joint_state_publisher`
- `joint_state_publisher_gui` (optional for GUI)
