# dual-arm-cable-insertion-ros2
Vision-assisted dual-arm cable handover and insertion using ROS 2, MoveIt 2 and ArUco-based pose estimation.
# Vision-Assisted Dual-Arm Cable Handover and Insertion using ROS 2 and MoveIt 2

## Overview

This project focuses on developing an autonomous dual-arm robotic system for cable handover and connector insertion.

The system is designed to use vision-based pose estimation to identify the cable and connector, coordinate two robotic arms, plan collision-free trajectories, perform an arm-to-arm cable handover, and execute precise insertion.

The project uses a low-cost 7-DoF bio-inspired robotic arm platform driven by serial-bus servos.

## Problem Statement

Cable insertion is challenging because the cable is flexible, its shape and tip orientation can change during manipulation, and the connector requires precise positioning and alignment.

A single robotic arm cannot simultaneously stabilize the cable and perform the insertion task. Therefore, the project uses coordinated dual-arm manipulation with an intermediate handover.

The two arms operate in a shared workspace, requiring collision-free planning between the arms, cable, and surrounding environment.

## Objectives

- Develop an ArUco marker-based vision system for estimating cable and connector poses.
- Implement dual-arm coordination using ROS 2 and MoveIt 2.
- Plan collision-free trajectories in a shared workspace.
- Perform autonomous cable handover and insertion.
- Validate the system through cable insertion and peg-in-hole tasks.
- Evaluate positioning accuracy, handover reliability, success rate, and execution time.

## System Architecture

The planned system consists of:

Vision System
        ↓
Pose Estimation
        ↓
ROS 2
        ↓
MoveIt 2
        ↓
Inverse Kinematics & Motion Planning
        ↓
Collision Checking
        ↓
Dual-Arm Manipulation
        ↓
Cable Handover & Insertion

## Technologies

- ROS 2
- MoveIt 2
- Python
- OpenCV
- ArUco Markers
- URDF / XACRO
- RViz
- Gazebo
- Motion Planning
- CAD
- Serial-Bus Servos

## CAD and Robot Design

The robotic arm was developed through iterative CAD design.

The first prototype was evaluated to identify mechanical and integration limitations. A redesigned prototype was developed to improve structural rigidity, workspace, precision, actuator integration and compatibility with ROS 2 and MoveIt 2.

## Current Status

**Project Status: In Development**

Current work focuses on:

- CAD completion
- URDF/XACRO robot modelling
- ROS 2 robot description
- MoveIt 2 integration
- Simulation and motion planning

Upcoming work includes:

- Dual-arm motion planning
- Vision integration
- Cable handover logic
- Cable insertion
- Hardware validation and testing

## My Contribution

I am involved in:

- Robotic arm CAD and mechanical design
- URDF/XACRO robot modelling
- ROS 2 integration
- Preparation for MoveIt 2-based simulation and motion planning
- Dual-arm robotic manipulation development

## Project Team

Alen George  
Bharath MS  
Rone Issac Biju  
Alen Francis

## Project Timeline

June 2026 – November 2026

## Project Documentation

Project presentation and supporting documentation are available in the `docs/` directory.

## Future Scope

- Marker-free cable and connector detection
- Cable shape estimation and tracking
- Force/tactile sensing for compliant insertion
- Learning-based handover and insertion
- Extension to multi-cable wiring-harness assembly
