# Husky_auto_navigation
Make Husky robot autonums

Veer Kalburgi

-------------------------------------------------------------

AUTONOMOUS ROBOT NAVIGATION USING ROS 
Clearpath Husky A200 robot navigation with Gazebo and RViz simulations using different SLAM and Path Planning algorithms. 360 degrees laser scan with two SICK LMS511 LIDARs.

------------------------------------------------------------- 
SIMULATION WORLD LAUNCH

$ roslaunch husky_gazebo husky_koridor3.launch

------------------------------------------------------------- 
RVIZ INTERFACE LAUNCH

$ roslaunch husky_viz view_robot.launch

------------------------------------------------------------- 
MANUAL DRIVE with PS3 JOYSTICK

$ roslaunch husky_control ps3_teleop.launch

-------------------------------------------------------------
AMCL 

Global Planners:
	A*
	Dijkstra
Local Planners:
	DWA
	TEB
	
$ roslaunch husky_navigation amcl_astar_dwa.launch 
---or---
$ roslaunch husky_navigation amcl_astar_teb.launch
---or---
$ roslaunch husky_navigation amcl_dijkstra_dwa.launch 
---or---
$ roslaunch husky_navigation amcl_dijkstra_teb.launch

-------------------------------------------------------------
