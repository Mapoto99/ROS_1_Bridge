# ROS_1_Bridge
## ROS_1_Bridge_Installation
### To create ROS1_Bridge do the following steps:
```
mkdir -p ~/ros1_bridge_ws/src
```
```
cd ~/ros1_bridge_ws/src
````
```
git clone https://github.com/ros2/ros1_bridge.git
```
```
cd ~/ros1_bridge_ws
```
```
rosdep update
```
```
rosdep install --from-paths src --ignore-src -r -y
```
```
colcon build --packages-select ros1_bridge
```
```
source ~/ros1_bridge_ws/install/setup.bash
```
## Running ROS_1_Bridge
### open two terminals:

#### in the first terminal type:
```
source /opt/ros/noetic/setup.bash
```
```
roscore
```
#### in the second terminal type:
```
source /opt/foxy/setup.bash
```
```
ros2 run ros1_bridge dynamic_bridge

```
