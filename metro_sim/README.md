Launch world:

```
roslaunch metro_sim terrain.world
```

Spawn Robot:

```
roslaunch metro_sim spawn_metro.launch
```

Issues:
* Robot flies away if spawn area is not clear of any obstacles. Remedy: Ensure world has a 'gap' in (0,0) xy pose for robot to spawn in.
