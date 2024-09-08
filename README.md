# wheeltec_ros2_driver

-Start the simulator by pressing F1 and selecting wokwi - start simulator

-Run the virtual_ports.sh shell script by typing ./virtual_ports.sh while in the root workspace

-launch the hardware interface: ros2 launch ar_hardware_interface stepper_hardware.launch.py

-launch the rviz application: ros2 launch ar_moveit_config ar_moveit.launch.py gripper_name:=wheeltec

**other relevant commands:**

View active socat instances:  ps aux | grep socat | grep -v grep

kill socat processes: kill <process id> or kill all instances: pkill socat

View running topics: ros2 topic list

View running nodes: ros2 node list

View running services: ros2 service list

View info on a service, node:  ros2 node info <node name>

View interface info:  example: ros2 interface show control_msgs/action/GripperCommand
