# NVIDIA-Visual-SLAM-
Aim
To compute the updated robot pose using motion displacement.
General Objective
To understand Visual SLAM (Simultaneous Localization and Mapping) and how incremental pose updates help track a robot’s position in an unknown environment.
Specific Objective
To compute the new pose using:
New Pose
=
Previous Pose
+
Motion
New Pose=Previous Pose+Motion
Given:
Previous Pose = (2, 3)
Motion = (0.4, 0.6)
Dataset
TUM RGB-D Dataset
Source: Technical University of Munich
Procedure
Input previous pose coordinates
Input motion displacement
Add corresponding values
Compute new pose
Display result
Algorithm
Start
Input previous pose 
(
x
,
y
)
(x,y)
Input motion 
(
d
x
,
d
y
)
(dx,dy)
Compute:
x
n
e
w
=
x
+
d
x
x 
new
​	
 =x+dx
y
n
e
w
=
y
+
d
y
y 
new
​	
 =y+dy
Display new pose
Stop
Code Logic
new_x = prev_x + dx
new_y = prev_y + dy
Python Code
# SESSION 14 – Visual SLAM (Pose Update)

# Step 1: Input previous pose
prev_x = 2
prev_y = 3

# Step 2: Input motion
dx = 0.4
dy = 0.6

# Step 3: Compute new pose
new_x = prev_x + dx
new_y = prev_y + dy

# Step 4: Display result
print("New Pose = (", new_x, ",", new_y, ")")

print("\nProgram Executed Successfully")
Output
New Pose = ( 2.4 , 3.6 )

Program Executed Successfully
Result
The updated robot pose is:
(2.4, 3.6)
Industry Application
Visual SLAM is used in:
Robotics navigation
Autonomous vehicles
AR/VR systems
Drone mapping
Companies like NVIDIA use this in:
Autonomous driving platforms
Robotics simulation
AI perception systems
Conclusion
Visual SLAM enables robots to track their position while building maps, and pose updates are fundamental to accurate localization.
