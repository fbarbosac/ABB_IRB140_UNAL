# ABB IRB 140 Gazebo

##Overview

This package contains the files required to simulate the ABB IRB 140  manipulator in Gazebo. 

Current version supports ROS Kinetic.


## Using Moveit! with Gazebo Simulator

1. Bring the robot model into gazebo and load the ros_control controllers:
   ```roslaunch abb_irb140_gazebo irb140_gazebo.launch``` 

2. Launch moveit! and ensure that it is configured to run alongside Gazebo:
```roslaunch abb_irb140_moveit_config moveit_planning_execution_gazebo.launch``` 
