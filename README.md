Package for BlueROV1 simulation.

The robot can be simulated either with Gazebo or UWSim rendering (`uwsim:=true` in launch files).

Control can be done either at the thruster or at the velocity level.

* Thruster control: `roslaunch bluerov_ffg thruster_cmd.launch`

  Once the robot is spawned in Gazebo, it waits for thruster inputs on `/brov/thruster_command` (JointState message using the effort field). By default a GUI is displayed to control the thruster inputs, it can be diabled by adding `gui:=false`.
  
* Velocity control: `roslaunch bluerov_ffg velocity_cmd.launch`

  This launch file runs Gazebo and also a PID control to map velocity setpoints to thruster commands. By default a GUI is displayed to give velocity setpoints, it can be diabled by adding `gui:=false`. The gains of the PID are in `config/brov.yaml`.

* To visualize the thruster forces: `roslaunch bluerov_ffg rviz.launch` 


