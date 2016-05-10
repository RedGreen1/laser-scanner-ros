# laserScannerROS
Program wrote using Robot Operating System. Visualize data from laser scanner. Independent from Rviz.

#Note
Program code is based on tutorials and examples available on http://wiki.ros.org/

# Note
In order to use this program you must have properly configured ROS (project wrote using Indigo version) on your PC. 
Then you have to create ROS package and put there files from repo.

# Usage
* In 1st terminal type: rosbag play bag/2016-04-27-09-47-12.bag - it will activate topick _scan_ wchich we are going to track.
* In 2nd terminal type: rosrun <package_name> listener
