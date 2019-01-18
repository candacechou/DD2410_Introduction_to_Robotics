# DD2410_Introduction_to_Robotics
1. Lab 2 : Inverse kinematic 
2. Lab 3 : Planning

	Installation

	git clone https://github.com/cisprague/dubins.git

3. Lab 4 : Mapping
	To run this, you have to open four terminals :
	
	Terminal 1: roscore
	
	Terminal 2: roslaunch mapping_assignment play.launch
	
	This launches RVIZ for you so that you can see how the robot moves and how the map is being updated by your code.

	Terminal 3: rosbag play --clock BAGFILE
	
	where 
	Argument    |	Purpose
	_______________________________________________________________________
       
       --clock	    | Publish the clock time. 
	            | This is to make sure that the time from 
		    |  the BAGFILE is published. Otherwise, 
		    |  the robot in RVIZ will not reset if you restart the bag.
        _______________________________________________________________________
	
	BAGFILE	    |  Path to a rosbag, which are located here 
		    |  mapping_assignment_metapackage/mapping_assignment/bags/

	Terminal 4: rosrun mapping_assignment main.py
