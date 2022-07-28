
### You want to control your robot ? take it step by step ! 👌 

Start by simulating the robot arm on your device. To do that, you need to follow some steps after downloading ROS on Ubuntu which I have explained in this repository: https://github.com/Razany98/ROS-Installation 

#####  Notes: The written commands below are for ROS noetic, so if you are using another distribution change the word 'noetic' to the one you are using. 

- #### 1 - The first thing you need to do is creating a workspace to install the arm package on it. 

Copy/Paste the following commands: 
  
- source /opt/ros/noetic/setup.bash 
- mkdir -p ~/catkin_ws/src (Here I named my workspace catkin_ws, you can choose it to whatever you want)
- cd ~/catkin_ws/
- catkin_make

Now you've created a workspace to put your arm package in. 

- #### 2 - Download the arm package
