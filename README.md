# ROS-GAZEBO-4-Mecanum-Wheel-Robot

This is a 4 mecanum wheel robot designed in SolidWorks then exported into URDF file using the SW to URDF ROS industrial package.
The objective is to create a Dynamic simulation of a 4 Mecanum Wheel Car Robot.

  It will respond realistically to forces and torques: accounting for mass, inertial, and friction.
  
  We want to command the robot's wheels with effort (torque), which is how real motor controllers work.
  
  We need to subscribe to ROS topics to read the robot's state in real-time, including its position , linear and angular velocity, and orientation (yaw angle).

How to launch the simulation in ubuntu VM terminal:
  Create ROS workspace:
    mkdir -p ~/catkin_ws/src
  Compile everything in the workspace:
    cd ~/catkin_ws
    catkin_make
  Source compiled files
    source devel/setup.bash
  Launch the simulation
    roslaunch omni_car_bot your_launch_file.launch
