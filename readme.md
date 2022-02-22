# FKIE Husky Manipulation Simulation 

## Description

The <code>fkie_husky_manipulation_simulation</code> package simulates a husky robot base and a manipulator arm such as a panda arm.

![example](readme_media/husky-panda-warehouse.png)

## Requirements
- Only ```franka_ros``` package needs to be installed from the source due to this [Issue](https://github.com/frankaemika/franka_ros/issues/218) in Melodic and Noetic. The husky related packages can be installed from the apt. 

## Launch files

- ```demo_*.launch```: Launches husky robot base with a panda arm in an empty environment or the two environments (warehouse and outdoor) used in the publication.
 
## Authors

```
Menaka Naazare 
menaka.naazare@fkie.fraunhofer.de

Francisco Garcia Rosas
francisco.garcia.rosas@fkie.fraunhofer.de

Fraunhofer FKIE 2022
```