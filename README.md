# RoboND_GoChaseIt
Submission for Project 2 of Udacity Robotics Nanodegree: robot design to locate and follow a white ball around a Gazebo world using ROS.

## Build and Run
This project is intended to be built within a [catkin workspace](http://wiki.ros.org/catkin/workspaces#Catkin_Workspaces). To build, clone this repo into the `catkin_ws/src` folder and run `catkin_make`.

After sourcing `setup.bash`, if not already:
```
$ roslaunch my_robot world.launch
$ roslaunch ball_chaser ball_chaser.launch
```
<img src="https://github.com/GeorgieChallis/RoboND_GoChaseIt/blob/master/my_robot/img/Rviz.png" width="640"/>

## Directory Structure
```
    .src                        
    ├── ball_chaser                  
    │   ├── launch
    │   │   ├── ball_chaser.launch   
    │   ├── src             	  
    │   │   ├── drive_bot.cpp         
    │   │   ├── process_image.cpp	
    │   ├── srv            	  
    │   │   ├── DriveToTarget.srv     
    │   ├── CMakeLists.txt      		  
    │   ├── package.xml     		  
    ├── my_robot                       
    │   ├── launch
    │   │   ├── robot_description.launch    
    │   │   ├── world.launch
    │   ├── meshes             	  
    │   │   ├── hokuyo.dae           
    │   ├── urdf
    │   │   ├── my_robot.gazebo
    │   │   ├── my_robot.xacro
    │   ├── worlds
    │   │   ├── simple-building.world 
    │   ├── CMakeLists.txt      		  
    │   ├── package.xml     		  
    ├── CMakeLists.txt                 
                             
```
