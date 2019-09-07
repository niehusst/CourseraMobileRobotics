# Assignment 6
This week you will be combining the go-to-goal, avoid-obstacles, and follow-wall controllers into a full navigation system for the robot. The robot will be able to navigate around a cluttered, complex environment without colliding with any obstacles and reaching the goal location successfully.

1. Implement the progress_made event that will determine whether the robot is making any progress towards the goal.
2. Implement the sliding_left and sliding_right events that will serve as a criterion for whether the robot should continue to follow the wall (left or right) or switch back to the go-to-goal behavior.
3. Implement the finite state machine that will navigate the robot to the goal located at (x_g,y_g)=(1.1,1.1) without colliding with any of the obstacles in the environment.


All the changes are in Supervisor.m
