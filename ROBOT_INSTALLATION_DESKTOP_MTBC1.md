## Manual installation of MockTurtleBotC1-Desktop packages on Desktop computer
### Refer to separate Manual Installation of MockTurtleBotC1-Robot on Desktop computer 

### Note: This Procedure installs navigation packages on the Desktop Computer (Ubuntu) that does has a connected monitor for robot, SLAM & Nav Visualization functions .      

### 1. Install Specfic Functional Packages from ROS 2 and MockTurtleBotC1-Desktop Github Repository

#### 1.1 Source your ROS2 distro and workspace
If it's your first time using ROS2 and haven't created your ROS2 workspace yet, you can check out 
[ROS2 Creating a Workspace](https://docs.ros.org/en/galactic/Tutorials/Workspace/Creating-A-Workspace.html) tutorial. 
The MockTurtleBotC1 code supports your_ros_distro = **humble** currently.

    source /opt/ros/humble/setup.bash
    cd <your_ws>
    colcon build
    source install/setup.bash

### 2. Download MockTurtleBotC1-Desktop and dependencies:

#### 2.1.2 Install MockTurtleBotcC1-Desktop package:
    
    cd mtbc1_ws
    git clone *https://github.com/ARLunan/MockTurtleBotC1-Desktop.git
*    rosdep update && rosdep install --from-path src --ignore-src -y 
    colcon build 
    source install/setup.bash
    

## Miscellaneous

