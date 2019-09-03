# DD2410_Introduction_to_Robotics
1. Lab 2 : Inverse kinematic 
	
	PART 1: SCARA ROBOT
	
	To visualize the robot, run: 
	
           roslaunch kinematics_assignment scara_launch.launch
	
	PART 2: KUKA ROBOT
	
	To visualize the robot, run: 

           roslaunch kinematics_assignment kuka_launch.launch
	
2. Lab 3 : Planning

	 // Dubins Car //
	 
	Installation

	   git clone https://github.com/cisprague/dubins.git
	
	To run your code :
	
	   python3 main.py
	   
	The code has been removed and put into the other repostory called 
	DD2410_Introduction_to_Robotics_mapping

3. Lab 4 : Mapping

	To run this, you have to open four terminals :
	
	Terminal 1: roscore
	
	Terminal 2: roslaunch mapping_assignment play.launch
	
	This launches RVIZ for you so that you can see how the robot moves and how the map is being updated by your code.

	Terminal 3: rosbag play --clock BAGFILE
	
	where :
	
        --clock:	       Publish the clock time. This is to make sure that the time 
			       from the BAGFILE is published.
			       Otherwise, the robot in RVIZ will not reset if you restart the bag.
	
       BAGFILE:	       	       Path to a rosbag, which are located  here: 
                               mapping_assignment_metapackage/mapping_assignment/bags/ 					
	
	
	Terminal 4: rosrun mapping_assignment main.py
