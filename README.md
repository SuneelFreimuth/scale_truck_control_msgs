# Scale Truck Control Messages

Custom ROS messages for [SuneelFreimuth/scale_truck_control](https://github.com/SuneelFreimuth/scale_truck_control/).

## Making Message Headers Available in Arduino IDE

If you do not already have a Catkin workspace, create one and build the message headers:
```
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/src
git clone https://github.com/SuneelFreimuth/scale_truck_control_msgs.git
cd ..
catkin_make
```

Assuming your Arduino sketchbook is located at `~/Arduino/`, run the following:
```
rosrun rosserial_client make_library.py ~/Arduino/libraries/ scale_truck_control_msgs
```

The headers will be installed at `~/Arduino/libraries/ros_lib/scale_truck_control_msgs/`
