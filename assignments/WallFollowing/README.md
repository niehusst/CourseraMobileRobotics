# Assignment 5
Implement a wall-following behavior mode to allow our hybrid automata robot to navigate convex and non-convex obstacles.

1. Compute a vector, u_{fw,t}_ that estimates a section of the obstacle ("wall") next to the robot using the robot's right (or left) IR sensors.
2. Compute a vector, u_{fw,p}_ , that points from the robot to the closest point on u_{fw,t}_.
3. Combine the two vectors, such that it can be used as a heading vector for a PID controller that will follow the wall to the right (or left) at some distance d_{fw}_
