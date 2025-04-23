# CDE2310 Grp 6 2425_S2
<p align="justify"> CDE2310 is a module under National University of Singapore (NUS) Innovation and Design Program (IDP). Also known as Fundamentals of Systems Design, it is a module focused on implementing the key methodologies of a systems engineering mindset, with an overall project goal of building a robot to complete tasks autonomously. This repository is proof of our team's hard work throughout the semester, and contains everything from our code bases to hardware and electrical schematics. </p>

## Setup
1. Follow the [ROBOTIS Turtlebot3 Quick Start Guide](https://emanual.robotis.com/docs/en/platform/turtlebot3/quick-start/) to setup both your [REMOTE PC] and [RPi]

2. Afterwards, ```git clone``` the repositories listed below into your ROS2 workspace
### File Structure
The resultant file structure should be as such
<pre>
[REMOTE PC]
2310_workspace/
├── launch_scripts
├── src/
│   ├── mission_control
│   ├── casualty_location
│   ├── aligner_node
│   ├── nav2_wavefront_frontier_exploration
│   └── custom_msg_srv
├── build/
├── install/
└── log/

[RPi]
2310_workspace/
├── src/
│   ├── turtlebot_launcher
│   ├── casualty_location
│   └── custom_msg_srv
├── build/
├── install/
└── log/
</pre>
- [launch_scripts](https://github.com/cde2310grp6/launch_scripts)
- [turtlebot_launcher](https://github.com/cde2310grp6/turtlebot_launcher)
- [mission_control](https://github.com/cde2310grp6/mission_control)
- [casualty_location](https://github.com/cde2310grp6/casualty_location)
- [aligner_node](https://github.com/cde2310grp6/aligner_node)
- [nav2_wavefront_frontier_exploration](https://github.com/cde2310grp6/nav2_wavefront_frontier_exploration)
- [custom_msg_srv](https://github.com/cde2310grp6/custom_msg_srv)

3. In ```2310_workspace``` run ```colcon build```
4. ```cd launch_scripts```
5. ```tmuxinator start 2310_mission_start```

Those are the basics, please refer to [launch_scripts](https://github.com/cde2310grp6/launch_scripts) for more launch parameters
and visit each repo for more info on their functions.


## Overview
The following is a simplified rqt_graph of the crucial nodes used in our project. It excludes the typical Nav2 Stack nodes, which are another key part of our robot's function.
![image](https://github.com/user-attachments/assets/630a5120-8ee0-498c-ba39-3ffd3cf99a92)


## Dependencies
- [ROS2 Humble](https://docs.ros.org/en/humble/index.html)
- [Nav2](https://docs.ros.org/en/humble/index.html)
- [Gazebo Classic 11.14.0](https://classic.gazebosim.org)
- Tmux
- Tmuxinator

## Acknowledgement
 - Special thanks to our CDE2310 Profs for organising this challenging yet fun module.
   - Mr Chew Wanlong, Nicholas
   - Mr Ee Wei Han, Eugene
   - Mr Royston Shieh Teng Wei
   - Mr Soh Eng Keng
 - Teaching Assistants of CDE2310
 - [SeanReg's Frontier Exploration algorithm](https://github.com/SeanReg/nav2_wavefront_frontier_exploration)
 - [Josh-Hrisko's amg8833 driver](https://github.com/makerportal/AMG8833_IR_cam)
 - Turtlebot3 Documentation 
 - [AniArka's Frontier Exploration algorithm (this should get a prize in code readability)](https://github.com/AniArka/Autonomous-Explorer-and-Mapper-ros2-nav2)
 - Don Pollo

##
Check out a [screen recording of our final run!](https://youtu.be/ttS_-xZGWaA)

![image](https://github.com/user-attachments/assets/9d3644fa-9304-4af6-8837-bdd32e732529)  
Thanks for reading!

