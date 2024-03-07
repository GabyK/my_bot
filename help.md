source /opt/ros/humble/setup.bash
source install/setup.bash

colcon build --symlink-install

ros2 launch my_bot launch_sim.launch.py

ros2 run teleop_twist_keyboard teleop_twist_keyboard