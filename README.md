# ROS2LaunchFile

ROS2 example: https://docs.ros.org/en/rolling/Tutorials/Launch-Files/Creating-Launch-Files.html

Requires ROS2 and turtlesim being installed to system

launnh: ros2 launch turtlesim_launcher.py 

send commands to sim1: ros2 topic pub -r 1 /turtlesim1/turtle1/cmd_vel geometry_msgs/msg/Twist "{linear: {x: 2.0, y: 0.0, z: 0.0}, angular: {x: 0.0, y: 0.0, z: -1.8}}"
(sim2 should follow the sim1 rotation)
