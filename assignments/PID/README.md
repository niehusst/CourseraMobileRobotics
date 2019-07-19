# Assignment 2

Implement a PID controller for a robot with go-to-goal behavior.
The location of the goal can be adjusted by editing the goal field of the `QBSupervisor` class.

1. Implement the proportional, integral, and derivative terms of the controller.
+simiam/+controller/GoToGoal.m
We need to keep track of previous state in order to calculate the integral over time.
Implement PID behavior in the `execute` function. It must compute the correct linear and angular velocity of the robot.
Compute the heading to the goal and the error the between that heading the robot's current heading. Save that error for the next run of the PID loop.

2. Adjust the gains for performance.
+simiam/+controller/GoToGoal.m

