# Engr005 Simulation Labs

## Dependencies
Ubuntu 20.04

[ROS noetic](http://wiki.ros.org/noetic)

If you have ros-noetic-desktop installed, the additional dependencies you must install are:

- tf2_geometry_msgs
- ackermann_msgs
- joy
- map_server

You can install them by running:
```
sudo apt-get install ros-noetic-tf2-geometry-msgs ros-noetic-ackermann-msgs ros-noetic-joy ros-noetic-map-server
```

## Installation 
To install the simulator package, clone the repo with the simulator and starter code into your catkin workspace:

```
mkdir -p ~/WHATEVER_ws/src
cd ~/WHATEVER_ws/
git clone https://github.com/baboonSTW/Engr005_Simulation_Labs.git
mv ./Engr005_Simulation_Labs/* ./src
rm -rf ./Engr005_Simulation_Labs
```
Then run catkin_make to build it:

```
cd ~/WHATEVER_ws
catkin_make
source devel/setup.bash
```

## Quick Start

To run the simulator on its own, run:

```
roslaunch f1tenth_simulator simulator.launch
```

This will launch everything you need for a full simulation; roscore, the simulator, a preselected map, a model of the racecar and the joystick server.