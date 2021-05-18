## Launch World
Launch demo world:
```
roslaunch metro_sim metro_demo.launch
```

Launch urban world [Citysim repo](https://github.com/osrf/citysim):
```
roslaunch city city.launch 
```


## Spawn Skid Steer Robot

Spawn Metro:
```
roslaunch metro_sim spawn_metro_ss.launch
```
Use rqt_robot_steering plugin to control robot:
```
rqt
```

## Others
### Creating world
Tips on creating own world through other modelling software eg. blender:
For creating own world using .dae file:
* Mimic file directory of [landscape example](https://github.com/nyangshawbin/gazebo_simulation/tree/master/metro_sim/worlds/landscape)
* Make sure folder can be found in: ${HOME}/.gazebo/models/
* Model can now be inserted into gazebo as model, or through [roslaunch](https://github.com/nyangshawbin/gazebo_simulation/blob/master/metro_sim/launch/landscape.launch) can be created for convenience. 

### Clearpath Husky
To use Husky, follow installation guide documented on [Clearpath Robotics Husky UGV Tutorials](http://www.clearpathrobotics.com/assets/guides/kinetic/husky/SimulatingHusky.html). 

Spawn Husky:
```
# Spawn Clearpath Husky
roslaunch husky_gazebo spawn_husky.launch

# Visualizing local point cloud
roslaunch husky_viz view_robot.launch
```
