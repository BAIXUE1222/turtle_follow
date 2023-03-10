# Auto-Police Catch Thief

This repository hosts the source code for the ROS turtle_follow package, which implements the `Auto-Police Catch Thief` game for the Robot Operating System (ROS) using Turtlesim.

![Short Game Play](docs/Auto-Police_Catch_Thief.gif)

## Usage
You can follow step by step guide in this link
https://drive.google.com/file/d/1k2nRjsfP7YS4K5GEtmAFx9mq6zSPqPml/view?usp=sharing

Or use the `turtle_follow` package, clone this repository into the `src` folder of your catkin workspace:

```console
baixue@ubuntuBx:~/catkin_ws/src$ git clone https://github.com/BAIXUE1222/turtle_follow.git
```

Then build the workspace with `catking-tools` or `catkin_make` and source the new package:

```console
# catkin-tools:
baixue@ubuntuBx:~/catkin_ws$ catkin build
# or use
baixue@ubuntuBx:~/catkin_ws$ catkin_make
# source your workspace using the setup.bash or setup.zsh depending on your shell
baixue@ubuntuBx:~/catkin_ws$ source devel/setup.bash
baixue@ubuntuBx:~/catkin_ws$ source devel/setup.zsh
```
It should be noted that if tf is not installed in your ROS, you need to install the `tf library` first

Finally, start `roscore`, run `turtlesim`, `turtle_follow_turtle_count` and `follow.launch`:

```console
roscore
rosrun turtlesim turtlesim_node
# open marks calculation terminal
rosrun turtle_follow turtle_follow_turtle_count  
# open Auto-Police Catch Thief programe
roslaunch turtle_follow follow.launch   
```

Note that each of the four commands above should be executed from another terminal so that it will run in its own process.


## ROS Node Graph

![rqt node graph](docs/rosgraph3.png)

## turtle_leader Node Graph Highlight
![rqt node graph](docs/turtle_leader_topic.png)

## Challenges Faced
- `Control algorithm design`
- `Coordination formula design`
- `Flocking and consensus algorithm implementation`

## Futurework Can be Done
This is the first release (version 0.0.0). The following features are planned, and contributions to them or new features and code improvements are welcome.

- `Advanced control algorithms`
- `Obstacle avoidance`
- `Apply flocking and consensus algorithms`
- `User interface`
- `Improve our knowledge and expertise in the field of robotics`
