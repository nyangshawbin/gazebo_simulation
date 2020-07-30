# Summary:

Follow installation guide documented on [Clearpath Robotics Husky UGV Tutorials](http://www.clearpathrobotics.com/assets/guides/kinetic/husky/SimulatingHusky.html). 


## Simulating Husky in Gazebo

Launch any world file with Husky Spawned, for eg.:
```
roslaunch husky_gazebo husky_empty_world.launch
```
or to use large outdoor environment such as [Citysim repo](https://github.com/osrf/citysim):
```
roslaunch city city.launch 
```

To spawn Husky robot:
```
roslaunch husky_gazebo spawn_husky.launch

Visualizing:
```
roslaunch husky_viz view_robot.launch
```

To use rqt_robot_steering plugin to control Husky. The . Run the rqt command, and select Plugins->Robot Tools->Robot Steering from the top menu:
```
rqt
```
