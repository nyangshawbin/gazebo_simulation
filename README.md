# Summary:

Follow installation guide documented on [Clearpath Robotics Husky UGV Tutorials](http://www.clearpathrobotics.com/assets/guides/kinetic/husky/SimulatingHusky.html). 


## Simulating World
To use large outdoor urban environment such as [Citysim repo](https://github.com/osrf/citysim):
```
roslaunch city city.launch 
```
For creating own world using .dae file:
* Mimic file directory structure of [landscape example](https://github.com/nyangshawbin/gazebo_simulation/tree/master/metro_sim/worlds/landscape)
* Make sure folder can be found in: ${HOME}/.gazebo/models/
* Model can now be inserted into gazebo as model, or a [roslaunch](https://github.com/nyangshawbin/gazebo_simulation/blob/master/metro_sim/launch/landscape.launch) can be created for convenience. 


## Simulating Robot (after loading world)

To spawn Husky:
```
roslaunch husky_gazebo spawn_husky.launch
```
Visualizing local point cloud:
```
roslaunch husky_viz view_robot.launch
```

To spawn Darpa robot:
```
roslaunch metro_sim spawn_metro.launch
```

Use rqt_robot_steering plugin to control any robot. Run 'rqt' command, and select Plugins->Robot Tools->Robot Steering from the top menu:
```
rqt
```
