## Compilation

### 1. Code
#### Static TF
```
<node pkg="tf" type="static_transform_publisher" name="<link_name>" 
        args="0.085 0 0.775 0 0 0 /<fram1> /<frame2> 100"/>
```
#### Launch file
```
<launch>
  <include file="$(find gazebo_ros)/launch/empty_world.launch">
    <arg name="world_name" value="$(find your_package_name)/worlds/your_world.world"/>
  </include>

  <param name="robot_description" command="$(find xacro)/xacro $(find your_package_name)/urdf/robot.urdf" />

  <node name="spawn_urdf" pkg="gazebo_ros" type="spawn_model" output="screen" args="-param robot_description -urdf -model my_robot -z 1"/>
</launch>

```
#### Unit test
```

    mkdir ~/catkin_ws/src -p
    cd ~/catkin_ws/src
    catkin_create_pkg tutorial rospy
    cd tutorial/
    mkdir test
    cd test/
    touch test_code.py
    chmod +x test_code.py
    ls

The content of our test_code.py file is:

#! /usr/bin/env python

import unittest
import rostest 


class MyTestCase(unittest.TestCase):
    
    def test_whatever(self):
        pass
    

if _name_ == "__main__":
    rostest.rosrun('tutorial', 'test_code', MyTestCase)

The first way of executing it is by calling it directly:
    ./test_code.py
```

### 2. Links
#### VNC Setup
```
vnc setup: http://mitchtech.net/vnc-setup-on-raspberry-pi-from-ubuntu/
```
#### VNC Fix
```
vnc fix: https://askubuntu.com/questions/1205687/ubuntu-18-04-vnc-grey-screen
```
#### RPi OS 64-bit
```
https://forums.raspberrypi.com/viewtopic.php?t=275370
```
#### USB Dongle RPi Setup
```
https://www.electronicshub.org/setup-wifi-raspberry-pi-2-using-usb-dongle/
```
#### Ubuntu 18.04 desktop on RPi
```
https://maker.pro/raspberry-pi/projects/install-ubuntu-18044-lts-on-your-raspberry-pi-board
```
#### ROS Key on RPi Fix
```
wget http://packages.ros.org/ros.key -O - | sudo apt-key add -
```

### 3. Repos
```
https://github.com/josephjoel3099/drone_sim.git
```
```
https://github.com/shannon112/IronFish
```

### 4. Videos


### 5. Products
