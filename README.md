# Industrial Robotics & Path Planning: Multibrand Trajectory Implementation
**Advanced KRL/V+ Programming, TCP Calibration & Industrial Process Control**

## Project Overview
This project focuses on the design, programming, and validation of complex robotic trajectories using two industry-leading platforms: **KUKA** and **Stäubli**. The objective was to implement high-precision movements for automotive welding and logistics pick-and-place cycles, ensuring optimal TCP (Tool Center Point) orientation and collision-free operation in industrial environments.

[Link to Demonstration Video: KUKA & Stäubli Workflows](#)

## Tech Stack
* **Industrial Robots:** KUKA VKR 125/1 (Automotive Series) & Stäubli TX60 (CS8 Controller).
* **Programming Languages:** V+ (VAL-II) and KRL (Kuka Robot Language).
* **Control Systems:** Teach Pendant.

---

## Project Case Study

### **Situation**
During my exchange at the **Universidad de La Rioja** and coursework at **BUAP**, I was tasked with developing production-ready routines for two distinct manufacturing scenarios: automotive welding simulation and high-speed component handling.

### Multi-Platform Robotic Cell


### **Task**
My objective was to master two proprietary languages (KRL and V+) to:
1.  **KUKA VKR 125/1:** Program a continuous 3D welding trajectory on a car door frame, maintaining a constant tool angle and velocity.
2.  **Stäubli CS8:** Design a robust pick-and-place cycle via serial terminal, optimizing motion blending and gripper synchronization.

### **Action**
To achieve professional-grade results, I implemented the following technical workflow:
1.  **Kinematic Configuration:** Performed 4-point TCP calibration and defined BASE coordinate systems to ensure spatial accuracy.
2.  **Logic Development (Stäubli):** Authored `prog3.pg` in **V+**, utilizing `APPRO` and `DEPARTS` commands for safe vertical transitions and `BREAK` for precise I/O triggering.
3.  **Path Optimization (KUKA):** Implemented a hybrid motion strategy using `PTP` for air-cut movements and `LIN` for the welding bead to maintain path integrity.
4.  **Debugging:** Utilized HyperTerminal for real-time monitoring of variables and iterative error correction of motion points.

### **Results**
* **Precision Validation:** Successfully executed a point welding trajectory on a non-linear car door geometry.
* **Cycle Efficiency:** Reduced idle time in the Stäubli pick-and-place cycle by optimizing motion blend radii between target points.
* **Legacy System Proficiency:** Demonstrated the ability to program industrial hardware via low-level serial interfaces (V+ Language).
* **Multibrand Competence:** Validated technical adaptability between industrial standards.

---

## Technical Documentation

### Implementation Methodology
* **KUKA VKR 125/1:** Focus on orientation control ($A4, A5, A6$ axes) to avoid singularities during the welding path.
* **Stäubli CS8:** Focus on I/O synchronization (`SIGNAL` commands) and trajectory clearance (`DEPARTS 200`).

## Repository Structure
* `/logic`: Text files with V+ and KRL scripts.
* `/media`: Robot path videos.

---
**Contact Information**
* **Diego Armando Soriano Sánchez** - [LinkedIn](https://www.linkedin.com/in/diego-soriano-eng/)
* **Email:** diegoarmando.sori@gmail.com
