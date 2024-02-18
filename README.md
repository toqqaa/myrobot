## **Required Installation** 
Install ROS Noetic: Follow the official ROS installation instructions for Ubuntu 20.04. You can find detailed instructions on the ROS website:

sudo apt update
sudo apt install ros-noetic-desktop-full

Initialize rosdep: Before you can use ROS, you will need to initialize rosdep, which enables you to easily install system dependencies for source you want to compile and is required to compile packages in a catkin workspace:


sudo rosdep init
rosdep update

Create a Catkin Workspace: Create a catkin workspace to build your ROS packages:


mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/
catkin_make

Install Navigation Stack and AMCL: The navigation stack includes packages such as move_base, map_server, and amcl. You can install these packages using the following command:


sudo apt install ros-noetic-navigation

## **Usage**

To clone this repository, execute the following command in your terminal:


cd yourcatkin_ws/src

git clone https://github.com/toqqaa/myrobot.git

cd myrobot



## **Gazebo Simulation**

roslaunch myrobot world.launch

## **RViz Visualization and Navigation**


roslaunch navigation navigation.launch 
