
### You want to control your robot ? take it step by step ! 👌 

Start by simulating the robot arm on your device. To do that, you need to follow some steps after downloading ROS on Ubuntu which I have explained in this repository: https://github.com/Razany98/ROS-Installation 

#####  Notes: The written commands below are for ROS noetic, so if you are using another distribution change the word 'noetic' to the one you are using. 

- #### 1 - The first thing you need to do is creating a workspace to install the arm package on it. 

Copy/Paste the following commands: 
  
- $ source /opt/ros/noetic/setup.bash 
- $ mkdir -p ~/catkin_ws/src (Here I named my workspace catkin_ws, you can choose it to whatever you want)
- $ cd ~/catkin_ws/
- $ catkin_make

Now you've created a workspace to put your arm package in. 

- #### 2 - Download the arm package: 

- $ git clone https://github.com/smart-methods/arduino_robot_arm.git  

the go to the catkin workspace you created by: $ cd ~/catkin_ws to install ROS dependencies: 
- $ rosdep install --from-paths src --ignore-src -r -y
- $ sudo apt-get install ros-noetic-moveit
- $ sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui
- $ sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher
- $ sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control
- $ sudo nano ~/.bashrc 
