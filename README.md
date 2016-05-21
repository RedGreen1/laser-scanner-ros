# laserScannerROS
Program uses Robot Operating System. Visualize data from laser scanner. Independent from Rviz.

#Tutorials
Program code is based on tutorials and examples available on http://wiki.ros.org/

# Note
In order to use this program you must have properly configured ROS (project made using Indigo version) on your PC. 
Then you have to create ROS package and put there files from repo.

# Build
* In your catkin workspace type _source ./devel/setup.bash_
* Create your_package according to http://wiki.ros.org/ROS/Tutorials/CreatingPackage
* cd to your_package
* Use here _git clone_ command
* go back to your catkin workspace and type _catkin_make_ to build program

# Usage with bag files
* In 1st terminal run _roscore_
* In 2nd terminal type: _rosbag play bag/2016-04-27-09-47-12.bag_ - it will activate topic _scan_ wchich we are going to track.
* In 3rd terminal type: _rosrun your_package listener_

# Usage with live scans
* Install hokuyo_node according to http://wiki.ros.org/hokuyo_node/Tutorials/UsingTheHokuyoNode
* In 1st terminal run _roscore_
* Plug in Hokuyo scanner and type: _rosrun hokuyo_node hokuyo_node_
* In 3rd terminal type: _rosrun your_package listener_
