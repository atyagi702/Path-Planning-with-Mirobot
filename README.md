# Path-Planning-with-Mirobot
# Manipulating 6-DOF Robotic Arm with Inverse Kinematics

This repository contains the complete path planning with Mirobot Manipulator arm. The project explores the design, modeling, control, and execution of trajectory-based manipulation tasks using a 6-DOF robotic arm and gesture-based control methods. The end goal is to **demonstrate joint-space and cartesian space path planning**, validated using **CoppeliaSim** and the **Mirobot platform**.

## Project Overview

The project is divided into 3 main tasks:

### Task 1: Kinematic Modeling
- Defined the modified Denavit-Hartenberg (mDH) table for a 6R-R robot arm.
- Built a simulation skeleton using CoppeliaSim, including collision boxes and a custom gripper model.
- Visualized the robot’s kinematic structure with and without an end-effector.

### Task 2: Joint Space Trajectory Planning

                            Video: Simulation-CoppeliaSim
https://github.com/user-attachments/assets/6a5e25c2-87b0-40a1-ad17-f23ca7cbb173

                            Video:Real Hardware-Mirobot
https://github.com/user-attachments/assets/46127940-1f65-459f-a2d3-a02c7a687bcb


- Defined a series of joint space key poses for the robot.
- Generated a smooth **quintic polynomial trajectory** through the waypoints.
- Simulated trajectory execution in CoppeliaSim and the physical Mirobot.
- Compared results against B-spline trajectories.

### Task 3: Inverse Kinematics

                        Video: Simulation-CoppeliaSim
https://github.com/user-attachments/assets/ea40dabe-563a-46b8-928b-0852f8004df5

                        Video: Real Hardware-Mirobot
https://github.com/user-attachments/assets/175f2ba6-5c11-44d2-b4cf-ca00771392a2


- Developed custom Newton-Raphson-based inverse kinematics solvers using Jacobian matrices.
- Compared different Jacobian formulations (6x6, 12x6, 4x6) and discarded non-optimal strategies.
- Implemented velocity and joint angle limit checks to ensure safe control.
- Plotted joint trajectories and validated accuracy.

## Demonstration Videos

-  **Trajectory Execution in CoppeliaSim**  
-  **Real-Time Execution on Mirobot**  
-  **Gift Box Placement Task**  

## Tools and Software Used

- **MATLAB Robotics Toolbox**  
- **CoppeliaSim (V-REP)**  
- **WLKATA Studio**  
- **Mirobot API and Control Tools**  
- **Custom Python & MATLAB scripts**

## Acknowledgements

This project was completed as part of the **Medical Robotics and Image-Guided Intervention** course at Imperial College London. Special thanks to the teaching assistants and faculty for providing resources and support.
