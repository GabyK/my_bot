source /opt/ros/humble/setup.bash
source install/setup.bash

colcon build --symlink-install

ros2 launch my_bot launch_sim.launch.py world:=./src/my_bot/worlds/obstacles.world

ros2 run teleop_twist_keyboard teleop_twist_keyboard

https://github.com/klintan/ros2_usb_camera
https://github.com/joshnewans/ros_arduino_bridge
https://github.com/YuLiHN/kinect2_ros2



#-------Dependencies--------

sudo apt install ros-humble-gazebo-ros2-control
