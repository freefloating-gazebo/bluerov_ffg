Package for BlueROV1 simulation.

Once the robot is spawned in Gazebo, it waits for thruster inputs on `/brov/thruster_command` (JointState message using the effort field).

# To launch Gazebo with a GUI to control the thrusters

 `roslaunch bluerov_ffg brov.launch`
 
 # To visualize the thruster forces
 
 `roslaunch bluerov_ffg rviz.launch` 
