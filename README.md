# tf_publisher_gui
Update Version of http://wiki.ros.org/tf_publisher_gui

## Description

The tf_publisher_gui is based on Martin Guenther's version.
It allows user to quickly adjust TF between two links. 
It's useful for building URDF or sensor alignment.

I add some convenience features for better usage.

Here is how it looks like my version:

# <img src="https://imgur.com/bfS1lDF.png">


## Features

- Select parent/child frame directly on the GUI
- Pre-load current TF when open the GUI
- Reset current TF by "Load Default" button
- Display roll/pitch/yaw both in degree and radius
- Add +/- button for better tuning. The default increment is 0.01m and 90 degree
- backward compatible with Martin's version 

## Install 
```
cd ~/catkin_ws/src
git clone https://github.com/mezl/tf_publisher_gui.git
cd ~/catkin_ws
catkin build
```

## Usage 
Remember to source your catkin_ws
```
soruce ~/catkin_ws/devel/setup.sh
```
Run with default frame
```
rosrun tf_publisher_gui tf_publisher_gui 
```

Run with pecify parent and child frame 
```
rosrun tf_publisher_gui tf_publisher_gui _parent_frame:=/base_link _child_frame:=/camera_link
```




## Video Demo
[![Alt text](https://img.youtube.com/vi/lWdfwoMgaT8/0.jpg)](https://www.youtube.com/watch?v=lWdfwoMgaT8)

