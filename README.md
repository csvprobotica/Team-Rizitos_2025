## RoboGenius WRO 2024
The RoboGenius team is integrated by Francis Mojica, Flor Glaize and Fiorella Campos, who represent Colegio San Vicente de Paúl, Santiago in this Future Engineers competition.

<div style="text-align: center;">
  <img src="https://github.com/csvprobotica/RoboGenius/blob/main/t-photos/RoboGenius-Normal.jpg" alt="Texto alternativo" width="400"/>
</div>

## Introduction
_In the future engineers competition, our robot must demonstrate its ability to solve specific technical challenges. This includes navigating an obstacle course and executing precisely programmed tasks. Our robot must complete the tasks autonomously and meet the challenges of this year 2024._

Engineering materials
====

This repository contains engineering materials of a self-driven vehicle's model participating in the WRO Future Engineers competition in the season 2024.

Materials to build our robot: [`list of electronic components`](https://github.com/csvprobotica/RoboGenius/blob/main/schemes/Listado%20de%20Componentes_2.png)
* 1 Lego Inventor Large Hub 88016
* 1 Rechargeable battery 7.4V 2100mAh
* 2 Medium Angular Motor 88018
* 2 Technic Distance Sensor 45604
* 2 Technic Color Sensor 45605


## Content
* [`schemes`](https://github.com/csvprobotica/RoboGenius/tree/main/schemes) contains a schematic diagram in JPG format of the electromechanical components illustrating all the elements (electronic components and motors) used in the vehicle and how they are connected to each other.
* [`src`](https://github.com/csvprobotica/RoboGenius/tree/main/src) contains code of control software for all components which were programmed to participate in the competition.
* [`t-photos`](https://github.com/csvprobotica/RoboGenius/tree/main/t-photos) contains 2 photos of the team (an official one and one funny photo with all team members).
* [`v-photos`](https://github.com/csvprobotica/RoboGenius/tree/main/v-photos) contains 6 photos of the vehicle (from every side, from top and bottom).
* [`video`](https://github.com/csvprobotica/RoboGenius/tree/main/video) contains the video.mp4 file with the robot driving demonstration.

## Mobility and Strategy of our Robot

<div style="text-align: center;">
  <img src="https://github.com/csvprobotica/RoboGenius/blob/main/v-photos/Robot.jpg" alt="Texto alternativo" width="400"/>
</div>

**Robot Description:**

Our robot is an innovative autonomous machine designed for navigation and obstacle avoidance in its environment. It is equipped with a series of sensors and motors that allow it to detect and respond to various stimuli along its path.

**Proximity Sensors:**
The robot features several strategically placed proximity sensors around its structure. These sensors enable the detection of walls and other obstacles, ensuring that the robot can navigate without collisions. The sensors work by measuring the distance to nearby objects and providing real-time data to the robot's control system.

**Motors:**
* Front Motor: This motor is responsible for the robot's turns. Upon receiving signals from the control system, it can rotate in different directions, allowing the robot to avoid obstacles and redirect its path.
* Rear Motor: This motor drives the robot forward. It is designed to provide smooth and consistent movement, adjusting as needed based on the navigation requirements determined by the sensors.

**Color Sensor:**
The robot is also equipped with a color sensor capable of detecting specifically red and green colors. When encountering a red or green object in its path, the robot's control system activates an evasion routine to avoid these objects, ensuring safe and uninterrupted navigation.

**Gyroscope Sensor:**
To enhance its navigation capability and ensure it follows a precise trajectory, the robot includes a gyroscope sensor. This sensor measures the robot's orientation and turns. The control system uses gyroscope data to perform up to three complete turns before stopping. This feature is essential for tasks requiring cyclical navigation or following specific patterns.

**Functionality:**
Together, these components allow the robot to navigate autonomously and efficiently in complex environments. Upon starting, the robot moves forward, using its proximity sensor to detect walls and adjust its trajectory through controlled turns by the front motor. Simultaneously, it monitors its surroundings for red and green objects to evade them. The gyroscope ensures the robot can make precise turns and count up to three turns before stopping, completing its operation cycle.


