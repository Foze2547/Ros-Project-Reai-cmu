# Ros-Project-Reai-cmu

colcon build --symlink-install

source install/setup.bash

ros2 launch articubot_one rsp.launch.py

ros2 run joint_state_publisher_gui joint_state_publisher_gui

ros2 launch articubot_one launch_sim.launch.py world:=path/to/123.world

ros2 run teleop_twist_keyboard teleop_twist_keyboard

ros2 launch gazebo_ros gazebo.launch.py

ros2 run gazebo_ros spawn_entity.py -topic robot_description -entity robot_name
