# FKIE Husky Manipulation Simulation 

## Description

The <code>fkie_husky_manipulation_simulation</code> package simulates a husky robot base and a manipulator arm such as a panda arm.

![example](config/media/husky-panda-warehouse.png)

## Requirements
This package has been tested on Ubuntu 20.04 and ROS Noetic with Gazebo 11.

## Installation
- Install dependencies:

```console
sudo apt install ros-noetic-franka-description ros-noetic-gazebo-ros-control ros-noetic-gazebo-ros-pkgs ros-noetic-husky-control ros-noetic-husky-description ros-noetic-jsk-rviz-plugins ros-noetic-ros-control ros-noetic-twist-recovery ros-noetic-dwa-local-planner ros-noetic-teb-local-planner ros-noetic-panda-moveit-config ros-noetic-mbf-costmap-nav ros-noetic-moveit-simple-controller-manager ros-noetic-global-planner
```

- Clone and build required packages:

```console
cd <your_ros_workspace>/src
git clone https://github.com/fkie/fkie_realsense_description
git clone https://github.com/fkie/realsense_gazebo_plugin
git clone https://github.com/fkie/fkie_behavior_trees
git clone https://github.com/fkie/fkie_husky_manipulation_simulation

catkin build
```
## Try it out!

The file ```demo_warehouse.launch``` launches husky robot base with a panda arm in an warehouse environment used in the RA-L [publication](https://ieeexplore.ieee.org/abstract/document/9695293).

```console
cd ros/
source devel/setup.bash
roslaunch fkie_husky_manipulation_simulation demo_warehouse.launch
```

Note: We highly recommend using [fkie_node_manager](https://github.com/fkie/multimaster_fkie/tree/master/fkie_node_manager) for starting and managing the ROS nodes. 

## Acknowledgements

Our work uses [husky robot](https://github.com/husky/husky) and the [panda arm](https://github.com/frankaemika/franka_ros) packages. 

Thanks to these [discussions](https://github.com/justagist/panda_simulator/discussions/44) and [Erdal's blog](https://erdalpekel.de/?p=55) for tips on panda arm integration with Husky robot in Gazebo.

All the gazebo simulation environments that were used for simulations in the [RA-L article](https://ieeexplore.ieee.org/abstract/document/9695293) and ICRA 2022 conference paper. The models are from [osrf/gazebo_models repository](https://github.com/osrf/gazebo_models).

## Authors

- Francisco J. Garcia R. [E-Mail](francisco.garcia.rosas@fkie.fraunhofer.de)
- Menaka Naazare - [E-Mail](menaka.naazare@fkie.fraunhofer.de)

## License

```
Copyright 2022 Fraunhofer FKIE

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
