# simple_2wd_robot
ROS packages related to control of a simple 2WD Arduino robot. See the [wiki](https://github.com/skohlbr/simple_2wd_robot/wiki) for further information.

![](https://github.com/skohlbr/simple_2wd_robot/wiki/images/simple_robot_img_small.jpg)

The following ROS packages are part of this repo:

* [simple_2wd_bringup](https://github.com/skohlbr/simple_2wd_robot/tree/master/simple_2wd_bringup) provides a launch file for starting up all onboard systems of the robot

* [simple_2wd_control_arduino](https://github.com/skohlbr/simple_2wd_robot/tree/master/simple_2wd_control_arduino) contains the controller that has to be flashed to the Arduino. From the root of your workspace use the following command for flashing:
```
rosrun simple_2wd_control_arduino upload.sh
```
* [simple_arduino_control](https://github.com/skohlbr/simple_2wd_robot/tree/master/simple_arduino_control) contains a node for translating standard ROS control commands (joy and cmd_vel) to commands for the Arduino.

* [simple_arduino_control_msgs](https://github.com/skohlbr/simple_2wd_robot/tree/master/simple_arduino_control_msgs) contains lightweight custom messages for communicating between ROS and the Arduino.
