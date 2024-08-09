# MPC approaches for collision free manipulator arm control

<img src=imgs/arm_mpc.gif height="300" width="300" > <p></p>
Figure 1: Linear Hierarchical MPC deployed in simulator.


<img src=imgs/mpc_robot.gif height="300" width="300" > <p></p>
Figure 2: Linear Hierarchical MPC deployed on the robot.

## Usage:
1) Install dependencies (required only for running this in ROS)-
Packages- First make sure you have [panda_simulator](https://github.com/justagist/panda_simulator/tree/noetic-devel); then clone this repository. 
Because we have edited the core files inside the panda simulator, it should be replaced by the copy attached in this repository. Thus rename the file rename_to_meam520_labs to meam520_labs. Now your robot will be able to run functions like ```set_joint_positions_velocities``` and ```set_joint_positions_velocities_torque```.

For the advanced user, we invite you to edit the ```interfaces.py``` file inside of the ```meam520_labs/core/``` folder.

2) Run this [file](/rename_to__meam520_labs/lib/final_project.ipynb)

<!-- ![rrt_algo](imgs/rrt_algo.png) -->

## Performance:
<img src=imgs/pandampc.png height="300" width="400" > <p></p>
Figure 3: Trajectory optimization using RRT and MPC

<img src=imgs/convex_set.png height="300" width="400" > <p></p>
Figure 4:  Defining obstacles as convex constraint

<img src=imgs/convergence.png height="300" width="400" > <p></p>
Figure 5: Convergence curve Heirarchial MPC (obstacle avoiding waypoints generated using RRT).

<img src=imgs/convergence_convex_set.png height="300" width="400" > <p></p>
Figure 6: Convergence curve for obstacle avoidance using MPC and convex sets.

<img src=imgs/statistics.png height="300" width="400" > <p></p>
Figure 7: Performance of MPC algorithm.

<img src=imgs/mpctestcases.png height="300" width="400" > <p></p>
Figure 8: Time taken by different control algorithms to manipulate robot (in seconds)

<img src=imgs/Joint_pos.png height="300" width="400" > <p></p>
Figure 9: Joint positions vs Time

<img src=imgs/Joint_vel.png height="300" width="400" > <p></p>
Figure 10: Joint velocities vs Time

<img src=imgs/Joint_accelerations.png height="300" width="400" > <p></p>
Figure 11: Joint accelerations vs Time