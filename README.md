# create workspace for the first time
mkdir -p ~/catkin_ws/src
cd ~/catkin_es/src
catkin_init_workspace

# compile
cd ~/catkin_ws
catkin_make

# environment variables
source /opt/ros/noetic/setup.bash
source ~/catkin_ws/devel/setup.bash
source ~/.bashrc

# create package
cd ~/catkin_ws
catkin_create_package planner

# put the code in planner/ and compile every time when you change the code

# run
roslaunch launch/main.launch


