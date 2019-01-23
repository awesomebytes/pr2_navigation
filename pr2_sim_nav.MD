# launch pr2 simulation with navigation

The workspace needs also pepper_virtual

git clone https://github.com/awesomebytes/pepper_virtual

# for a world with nothing
roslaunch pr2_navigation_slam pr2_no_arms_empty_world.launch

# for a world with a little office map
roslaunch pr2_navigation_slam pr2_no_arms_office.launch

# if you want to do mapping
roslaunch pr2_navigation_slam slam_gmapping.launch

# launch the move_base (has no local costmap / safety)
roslaunch pr2_navigation_global move_base.launch


# to move around by hand

rosrun rqt_robot_steering rqt_robot_steering

