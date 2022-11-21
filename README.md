# turtlebot3 particle filter localisation

## Description:
I implemented the particle filter localisation algorithm within a ROS workspace on the turtlebot3 in the gazebo simulation environment. This enables the robot to determine its position in any map using observations of the world. 

The assignment was separated into 5 tasks that correspond with the 5 main steps of the particle filter algorithm. First, initialized the particles then normalize the weights, perform a motion update, perform an observation update, and then estimate the pose of the robot. In execution this is an iterative process wherein the steps are repeated over and over. 

![grafik](https://user-images.githubusercontent.com/115760050/202967667-82121a83-f136-4908-8dfa-1112b745442c.png)

Video demonstration: https://youtu.be/9-Ic-UhGuHQ

## Challenges:
- High computational requirements (depending on #particles and ROS Subscriber queue size)
- Unwanted outcomes due to probabilistic nature of algorithm (especially when a map contained similar looking sections)
