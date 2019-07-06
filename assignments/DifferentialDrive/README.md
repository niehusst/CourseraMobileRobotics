# Assignment 1

Add movement capability to the differential drive robot in the Sim.I.am robot simulator.

This is done by:
1. adding interpretation ability of the IR sensor data feedback
Implement code that converts raw IR values to distances (in meters).
Code in +simiam/+robot/QuickBot.m

2. converting unicycle model variables to differential drive model input
Implement the transformation from unicycle dynamics to differential drive dynamics, i.e. convert from (v,ω) to the right and left angular wheel speeds (vr,vl).
Code in +simiam/+robot/+dynamics/DifferentialDrive.m

3. Using wheel encoders to give robot some knowledge of its location in the world
Implement odometry for the robot, such that as the robot moves around, its pose (x,y,θ) is estimated based on how far each of the wheels have turned. Assume that the robot starts at (0,0,0).
Code in +simiam/+controller/+quickbot/QBSupervisor.m
