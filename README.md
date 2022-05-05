# gmapping_lms11_without_odom
gmapping_lms11_without_odom
# hector_slam_lms11
Gmapping slam on sick safety scanner lms11
Terminal 1:
LAUNCH THE LMS11 SENSOR NODE 
user:~/test_ws/
source /opt/ros/melodic.setup.bash
catkin build or catkin_make
source ./devel/setup.bash
roslaunch slam_test lms11.launch 

Terminal 2:
LAUNCH THE GMAPPING NODE in BRINGUP PACKAGE 

user:~/test_ws/
source /opt/ros/melodic.setup.bash
catkin build or catkin_make
source ./devel/setup.bash
roslaunch bringup mappings.launch

Terminal 3:
OPEN RVIZ AND ADD map,laser scan to view the map 

user:~/test_ws/
source /opt/ros/melodic.setup.bash
catkin build or catkin_make
source ./devel/setup.bash
rosrun rviz rviz

Links to follow 
https://github.com/ros-perception/slam_gmapping
http://wiki.ros.org/LMS1xx
https://github.com/clearpathrobotics/LMS1xx/tree/melodic-devel
add everything as submodule and make a change on it
sudo apt-get install ros-melodic-gmapping
sudo apt-get install ros-melodic-slam-gmapping 
sudo apt-get install ros-melodic-lms1xx
