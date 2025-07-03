## Team Rizitos WRO 2024

We are **Team Rizitos**, a robotics team competing in the **Future Engineers Senior's category of the WRO**. Our group is made up of two seniors, **Flor Glaize and Francis Mojica** , and one junior, **Hebe Hernández**. Together, we combine creativity, teamwork, and technical skills to bring our robot to life.
Our robot, also named **Rizitos**, is designed to complete 3 laps and overcome a variety of obstacles in the WRO Future Engineers Senior's course. We proudly represent **Colegio San Vicente de Paúl from Santiago de Veraguas, Panamá**.



Engineering materials
====

This repository includes all the engineering materials we used to build our robot, Rizitos, for the 2025 season of the WRO Future Engineers competition.

Below is the list of parts we used to assemble our self-driving vehicle:

Materials to build our robot: [`list of electronic components`](https://github.com/csvprobotica/RoboGenius/blob/main/schemes/Listado%20de%20Componentes_2.png)
* 1 Lego Inventor Large Hub 88016
* 1 Rechargeable battery 7.4V 2100mAh
* 2 Medium Angular Motor 88018
* 2 Technic Distance Sensor 45604
* 2 Technic Color Sensor 45605


Building Instructions
====
* **Robot Structure:**
  - The main idea of  Rizito’s design was developed by us and a source that  we used as a guideline .[`M.V.P`](https://osoyoo.com/manual/sportcarkit.pdf)


## Content
* [`schemes`](https://github.com/csvprobotica/RoboGenius/tree/main/schemes) contains an explanatory  diagram in PNG format of the electromechanical components illustrating all the elements (motors, sensors ,etc.) with its connections.
* [`src`](https://github.com/csvprobotica/RoboGenius/tree/main/src) this record contains all Rizito's Arduino code programming ( which is text-based style) that makes our robot move.
* [`t-photos`](https://github.com/csvprobotica/RoboGenius/tree/main/t-photos) you'll find Rizito's Team members  official photo.
* [`v-photos`](https://github.com/csvprobotica/RoboGenius/tree/main/v-photos) in this folder you'll encounter our robot, Rizitos, from 6 different angles.
* [`video`](https://github.com/csvprobotica/RoboGenius/tree/main/video)  the video shows Rizitos in action, where it completes the whole 3 laps.

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


