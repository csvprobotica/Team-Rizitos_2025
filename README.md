
</p>

<h1 align="center">Team Rizitos 🇵🇦 — WRO Future Engineers 2025</h1>
<p align="center">
  <i>Panamá • WRO FUTURE ENGINEERS SENIOR'S CATEGORY • Modular Robotics System • Block-Based Code</i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Custom%20Chassis-20C997?style=flat-square"/>
  <img src="https://img.shields.io/badge/Language-mBlock%20(Block%20Code)-20C997?style=flat-square"/>
  <img src="https://img.shields.io/badge/Team-Colegio%20San%20Vicente%20de%20Paúl-ADB5BD?style=flat-square"/>
</p>

---

##  Introduction

We are **Team Rizitos**, a student robotics team from *Colegio San Vicente de Paúl* in Santiago, Veraguas 🇵🇦.  
Our group includes two seniors — **Flor Glaize** and **Francis Mojica** — and one junior, **Hebe Hernández**.

Together, we combine creativity, logic, and persistence to bring Rizitos to life: a fully autonomous robot designed to overcome obstacles, complete multiple laps, and finish strong.

---

##  Our Robot: **Rizitos**

<p align="center">
  <img src="https://github.com/csvprobotica/Team-Rizitos_2025./blob/main/v-photos/v3./front.jpeg"/>
</p>

**Rizitos** is our autonomous self-driving robot which is designed to complete 3 laps and overcome a variety of obstacles in the WRO Future Engineers Senior's course.

The robot is based on a custom-modified chassis and multi-sensor platform. It includes distance detection, turning logic, lap tracking, and precise stop behavior — all coded in **mBlock**, running fully offline on a modular robotics controller.

---

##  Meet the Minds Behind Rizitos!

<table align="center">
  <tr>
    <td colspan="3" align="center">
      <img src="https://github.com/csvprobotica/Team-Rizitos_2025./blob/main/t-photos/WhatsApp%20Image%202025-07-03%20at%2007.42.20.jpeg" width="80%" alt="Team Rizitos Group Photo"/>
    </td>
  </tr>
  <tr>
    <td align="center">
      <b>Hebe Hernández</b><br>
      Rizito's Documenter 📄<br>
      <sub>Records Rizito's GitHub repository, diagrams and schemes</sub>
    </td>
    <td align="center">
      <b>Francis Mojica</b><br>
      Rizito's Software Programmer 💻<br>
      <sub>Creates Rizito's coding and programming</sub>
    </td>
    <td align="center">
         <b>Flor Glaize</b><br>
      Rizito's Mechanical Builder ⚙️<br>
      <sub>Focuses on Rizito's structure and hardware</sub>
    </td>
  </tr>
</table>

---

##  Repository Content

This is Rizito's Repository Index, where it shows all steps for Rizito's creation!:

| Folder          | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| [`models/`](./models)     | Contains Rizito's STL and design files used for 3D printing and fabrication.        |
| [`schemes/`](./schemes)   | PNG diagrams illustrating all electromechanical components and wiring connections. |
| [`src/`](./src)           | Source code programmed in mBlock that controls the robot's autonomous functions.   |
| [`t-photos/`](./t-photos) | Official team group photo of Team Rizitos.                                         |
| [`v-photos/`](./v-photos) | Photos of Rizitos robot taken from multiple angles.                               |
| [`video/`](./video)       | Final challenge video of Rizitos completing all 3 laps.                           |

---

##  Engineering Materials

Below is a summary of the core components used to bring Rizitos to life. All parts were assembled and modified by us to meet the WRO Future Engineers 2025 challenge.

- Smart Robotics Controller Hub (ID: 88016) – Rechargeable 7.4V, 2100mAh  
- 2x Medium Angular Motors (ID: 88018) – One for forward movement, one for steering  
- 2x Distance Sensors (ID: 45604) – For frontal and side obstacle detection  
- Internal Gyroscope Sensor – Used to measure orientation and track laps  
- Modular chassis built with pin-connected structural elements  

---

##  Building Instructions

**Robot Structure:**
- The main concept for Rizitos' design was developed by our team using structural and mechanical logic from modular robotics platforms.

**Operating Diagram:**
- The [`schemes/`](./schemes) folder contains all diagrams used to distribute Rizito's connection ports and lists all electronic components.

**Programming Code:**
- The [`src/`](./src) folder includes our block-based mBlock code that manages the robot’s movement, sensors, and decision-making logic.

>  *All programming and hardware integration were done by ourselves.*

>  **Rizitos is in constant evolution!.**  
> As we iterate, test, and improve our system, both the software and hardware may be updated regularly.  
> If you notice inconsistencies between sections or media, feel free to reach out or contribute!

---

## Rizito's Mobility System

### Key Functional Behaviors

#### 1. **Continuous Forward Movement**
- The robot uses a **Medium Angular Motor (ID: 88018)** in the rear to drive forward.
- The **front-facing Distance Sensor (ID: 45604)** continuously monitors for obstacles ahead.

#### 2. **Lateral Obstacle Detection & Evasion**
- A second **Distance Sensor (ID: 45604)** is mounted at an angle for lateral scanning.
- When an obstacle is detected:
  - The rear motor halts.
  - The **front Medium Angular Motor (ID: 88018)** turns the chassis left or right.
  - Once the path is clear, forward motion resumes.

#### 3. **Turning and Steering**
- The robot uses a front-mounted **Medium Angular Motor (ID: 88018)** for steering.
- It receives directional commands based on sensor feedback.
- After completing the turn, the motor resets to its center position for straight movement.

#### 4. **Lap Completion and Stop Behavior**
- The robot keeps track of laps internally using a built-in **gyroscope sensor**.
- After completing **3 full laps**, it:
  - Deactivates the rear motor.
  - Centers the steering motor.
  - Stops at its starting position and remains idle.

---

###  Why These Components?

| Component                       | Purpose & Reason                                                                  |
|--------------------------------|-----------------------------------------------------------------------------------|
| **Medium Angular Motor (x2)**  | One drives forward motion, the other controls turning and steering.              |
| **Distance Sensor (x2)**       | Detects nearby obstacles both ahead and to the side.                             |
| **Gyroscope Sensor**           | Measures orientation and turns; tracks lap completion.                           |
| **Smart Controller Hub**       | Central unit that powers and processes all components.                           |

---

## 🧭 Navigation Strategy

The code we developed for Rizitos enables it to function **fully offline** and autonomously complete its WRO Future Engineers tasks — from open-lap circuits to obstacle-filled tracks. Using mBlock and our modular platform, our logic adapts in real-time to environment conditions, enabling dynamic movement, evasive maneuvers, and consistent loop tracking.

---

###  Open Round Strategy (No Obstacles)

In the Open Round, Rizitos focuses on uninterrupted movement and precise tracking of lap completions:

1. **Initialization**
   - The system powers up and configures all key ports.
   - Motors and sensors are initialized.

2. **Lap Execution**
   - The **rear motor** pushes the robot forward.
   - The **steering motor** is fixed in its neutral center alignment.
   - A lap counter keeps track of completed loops using gyroscopic orientation.

3. **Stop Condition**
   - After three full laps, the motor is stopped.
   - Rizitos halts and re-centers its motors.

---

###  Obstacle Round Strategy (Dynamic Avoidance)

In the Challenge Round, Rizitos switches to a reactive navigation strategy using distance sensing and steering logic:

1. **Active Scanning**
   - The **distance sensors** monitor the robot’s surroundings.
   - Obstacle detection occurs continuously via distance sampling.

2. **Obstacle Encounter Logic**
   - If an object is detected ≤15cm ahead:
     - **Forward motion stops**
     - The robot chooses the clearer path based on lateral sensor readings.
     - The **steering motor** turns the wheels accordingly.
     - The robot resumes forward movement.

3. **Gyroscopic Orientation**
   - A **gyroscope module** measures orientation and rotation.
   - The lap counter checks for three full turns to confirm course completion.

4. **Completion Behavior**
   - After the third full lap (with successful evasion logic), the system cuts motor power and resets motors.
   - Rizitos comes to a full and final stop at its original point.

> This reactive planning system enables Rizitos to perform autonomously without AI inference or remote control!

---

**Rizitos is not just a robot — it’s a reflection of our team’s collaboration, growth, and effort.**  
Every wire connected, every block of code arranged, and every obstacle overcome was a result of three people working as one.

We are proud of what we’ve built — not just Rizitos, but the experience and bond that came with it.  
And we’re even more excited to share it with the world!

> If you have questions or want to share your thoughts, feel free to do so through the GitHub comments!



