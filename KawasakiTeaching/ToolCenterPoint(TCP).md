# Kawasaki robot tool center point teaching (TCP)
## AS Language programming
### HERE commands
We know from the Kawasaki manual, that we can use HERE commands in the terminal to teach the Tool Center Point (TCP).

<img src="https://github.com/larsn84/KawasakiRobot/blob/7eb75734a953bf1d028c21a3efa961cbdfdf4413/raw_images/TCP_HERE_commands.png" width="350"> 

1. It is recommended to use ```TOOL NULL``` the first time, unless you are sure 
2. ```HERE a``` defines the distance from the robots base coordinates (0,0,0) to the flange of the robot arm, when the robot is in position. This transfers the current coordinates to the "a" variable.
3. ```HERE a+b``` defines the distance from the robots base coordinates to the TCP (where we want our robot to grab the objects). This can be between two grippers, in center of a vacuum cup or whatever needed.
4. By typing ```POINT t=-b``` we assign the tool transformations values from b
5. ```TOOL t``` can be used to "mount" the new tool
   **Use ```DO ALIGN``` to align the robot to the workplane**
## Manuel Numeric Entry

## Automatic Tool registration
