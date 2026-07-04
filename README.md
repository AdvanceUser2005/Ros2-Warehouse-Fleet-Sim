# ROS 2 Warehouse Fleet Simulation

A production-style robotics software project that simulates autonomous warehouse robots performing task execution, navigation, obstacle avoidance, robot health monitoring, and fleet telemetry.

## Project Status

**Status:** In Progress  
**Current Milestone:** Building ROS 2 simulation + robot task manager  
**Planned:** AWS-based fleet telemetry dashboard

## Why I Built This

Warehouse robotics systems require more than just robot movement. They need reliable autonomy, task execution, monitoring, logging, and fleet-level visibility. This project is designed to practice the kind of robotics software patterns used in production robot systems.

## Features

- ROS 2-based warehouse robot simulation
- Autonomous navigation using Nav2
- Custom ROS 2 nodes/services for mission control
- Robot state reporting and health monitoring
- Fleet telemetry architecture for pose, battery, task state, and errors
- Dockerized development environment
- Planned AWS-based monitoring backend

## Tech Stack

- ROS 2 Humble/Jazzy
- C++ / Python
- Gazebo / Isaac Sim
- Nav2
- Linux / Docker
- CMake
- AWS IoT Core, Lambda, DynamoDB, S3, CloudWatch *(planned)*

## System Architecture

```text
Warehouse Robot Simulation
        |
        v
ROS 2 Navigation Stack
        |
        v
Task Manager Node
        |
        v
Robot State / Health Monitor
        |
        v
Telemetry Publisher
        |
        v
Fleet Dashboard / AWS Backend