# Assignment 3
This assignment is to make a controller that steers the robot successfully away from obstacles to avoid a collision. The IR sensors allow us to measure the distance to obstacles in the environment, but we need to compute the points in the world to which these distances correspond. 

We must:
1. Transform the IR distances to points in the world.
This is done by a series of translations and rotations with an R matrix;
[[ x_w ]=R(x_r,y_r,theta_r)*R(x_s,y_s,theta_s)*[[ d ] 
 [ y_w ]                                        [ 0 ]
 [  1  ]]                                       [ 1 ]]
2. Compute a vector to each point from the robot
3. Weigh each vector according to their importance

For example, the front and side sensors are typically more important for obstacle avoidance while moving forward.
Sum the weighted vectors to form a single vector
Use this vector to compute a heading and steer the robot to this heading.

This strategy will steer the robot in a direction with the most free space (i.e., it is a direction away from obstacles).

Implemented in this assignment:
1. Transform the IR distance (which you converted from the raw IR values in Week 2) measured by each sensor to a point in the reference frame of the robot.
2. Transform the point in the robot's reference frame to the world's reference frame.
3. Use the set of transformed points to compute a vector that points away from the obstacle. The robot will steer in the direction of this vector and successfully avoid the obstacle.
