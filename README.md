# Motoman_AIMS

An developmental application of ROS-Industrial for Yaskawa Motoman robots.

### Background

AIMS Lab. Gazebo Simulation of Motoman Robots using ROS Industrial. Melodic + Dashing.

This package is forked from the original motoman package kinetic devel, preserving only packages of interest. The motoman_mh5_support package's urdf/xacro files were modified to allow Gazebo-9 simulation. Additionally, modifications were implemented to allow interaction with the FS100 controller I/O's.

This metapackage contains packages developed by the ROS-I project.

### Usage
This package is designed as the complete contents of the <workspace>/src folder of a ROS1 workspace built using [catkin tools](https://catkin-tools.readthedocs.io/en/latest/#).
<br>Utilize the following commands to prepare a ROS workspace. We will assume that the workspace name is `ws_core`.
  
    mkdir -p ~/ws_core/src
    cd ws_core
    catkin init
    cd src

### Features / Capability
- Base MH5 ROS control
- Moveit integration w/ MH5 Robot
- IO pin control of FS100 controller. (other controllers untested to date)
- Rviz visualization (via moveit plugin) of MH5 robot
- Gazebo Simulation of MH5
