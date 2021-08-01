# Using-SLAM-map-to-launch-the-navigation
Using SLAM map to launch the navigation
#pre Requirements:
* Ubuntu 
* ROS
```
NOTE : I used ROS melodic 
```


# Steps;

* step1- You need to instal ROS package + Turtlebot3 Package
* step2 - after install the dependencies,you need to create and save the Turtlebot map Using SLAM
* step3- launch the navigation.

# Navigation Simulation:
* dependencies : 

```
 export TURTLEBOT3_MODEL=burger
 roslaunch turtlebot3_gazebo turtlebot3_world.launch
```
* Open a new Terminal :

```
 export TURTLEBOT3_MODEL=burger
 roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml
 ```
 * Open a new terminal to control the robot :
 
 ```
 roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch
 ```
 
 ![slam](https://user-images.githubusercontent.com/86341464/127772272-609c2e9c-29fd-4d14-a93a-31ba95c558a5.PNG)

 # source:
  https://emanual.robotis.com/docs/en/platform/turtlebot3/nav_simulation/
