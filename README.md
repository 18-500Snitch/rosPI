# ROS PI
## ROS Packages:
* rplidar\_ros
* hector\_slam_

### [rplidar\_ros](http://wiki.ros.org/rplidar)
#### Brief:
  ROS interface to rplidar\_sdk
#### Launch:
  Unplug than replug RPLIDAR USB
```
roslaunch rplidar_ros rplidar.launch
```
#### Close:
```
C-c
```
#### Modifications:
  - uses USB-rules namings
### [hector\_slam](http://wiki.ros.org/rplidar)
#### Brief:
  Simultaneous Localization and Mapping (no need for odometry)
#### Launch:
```
roslaunch hector_slam_launch tutorial.launch
```
#### Close:
```
C-c
```
#### Modifications:
  - Changes made to bypass optional odometry frame.

## TODO:
- [x] catkin\_make
- [x] test SLAM and RPLIDAR separate from quadcopter 
  - works until angle change too great
- [ ] send RPLIDAR data to python code via sockets for navigation purposes
- [ ] test SLAM and RPLIDAR mounted on quadcopter
- [ ] fine tune arguments/parameters
- [ ] _integrate Pixhawk odometry data for better mapping_
- [ ] _integrate range finder for 2.5D mapping_
