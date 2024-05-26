## Compilation

### 1. Code
#### Static TF
```
<node pkg="tf" type="static_transform_publisher" name="l515_depth_link" 
        args="0.085 0 0.775 0 0 0 /base_link /l515_optical_link_depth_frame 100"/>

  <node pkg="tf" type="static_transform_publisher" name="l515_depth_link_link"
        args="0 0 0 0 0 0 /base_link /l515_optical_link_link 100"/>
```
#### ROS Key on RPi Fix
```
wget http://packages.ros.org/ros.key -O - | sudo apt-key add -
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

### 3. Repos
```
https://github.com/josephjoel3099/drone_sim.git
```
```
https://github.com/shannon112/IronFish
```

### 4. Videos


### 5. Products
