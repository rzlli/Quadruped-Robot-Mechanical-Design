# Mechanical Design of a Quadruped Robot Dog
## Cooperative Training Program - Smart Methods

This repository contains the mechanical analysis and initial design documentation for a simple quadruped robot dog. The model was designed using Tinkercad to study the core mechanical concepts required for standing, stability, and locomotion.

---

##  Design Details & Mechanical Analysis

### 1. Body and Frame 
* Structure: The robot consists of a rectangular body frame equipped with four legs.
* Function: The frame provides robust structural support to house and hold all components, controllers, and power sources.

### 2. Leg Design
* Structure: Each leg is designed with three segments connected by three joints:
  * Hip Joint: Located at the connection of the leg to the body.
  * Knee Joint: Located at the middle of the leg segment.
  * Ankle/Foot Joint: Located at the foot interface.

### 3. Joints and Degrees of Freedom 
The robot's degrees of freedom (DOF) are structured as follows:

| Joint | Per Leg | Total (4 Legs) |
| :--- | :---: | :---: |
| Hip Joint |  1 DOF | 4 DOF |
| Knee Joint  | 1 DOF | 4 DOF |
| Ankle/Foot Joint |   1 DOF | 4 DOF |
| Total DOF  |3 DOF | 12 DOF |

$$\text{Total DOF} = 4\text{ Legs} \times 3\text{ DOF} = 12\text{ DOF}$$

### 4. Motor Selection 
* Actuator: MG996R Servo Motor.
* Configuration: One high-torque servo motor is dedicated to driving each individual joint, providing precise control over the leg segments.

### 5. Basic Torque Calculation 
To determine the required motor performance, the joint torque ($\tau$) is calculated as follows:

* Formula:

$$\tau = F \times r$$

Where:
* $\tau$ = Torque 
* $F$ = Force 
* $r$ = Distance from the joint 

* Calculation:
Assuming:
  * $F = 2.94\text{ N}$
  * $r = 0.1\text{ m}$

$$\tau = 2.94 \times 0.1 = 0.294\text{ N}\cdot\text{m}$$

* Result: The required joint torque is approximately $0.3\text{ N}\cdot\text{m}$.

### 6. Stability and Center of Gravity 
* Alignment: The center of gravity (CoG) is located at the center of the robot's body.
* Stability: This central placement of weight improves overall balance and static stability.

### 7. Walking Gait 
* Gait Type: Alternating Walking Gait 
* Mechanism: The robot moves using a natural alternating leg gait (diagonal pairs or alternating sequences). This allows the robot to advance smoothly and naturally, mimicking a real dog's walk, while maintaining dynamic balance throughout the movement.

### 8. Expected Mechanical Problems 
* Joint Friction: Mechanical friction in the moving joints.
* Balance Loss: Potential loss of balance during dynamic leg movements.
* Slipping: Slipping of the legs on smooth surfaces.

---

##  Repository Structure
* Tinkercad_Robot_Design.png: A single comprehensive screenshot of the robot dog design created within Tinkercad.
* Mechanical_Design_Analysis.png: The comprehensive infographic diagram showcasing the layout, summary report, joint configurations, and torque calculations.
* * ingenious_Wluff.stl: The 3D file format of the robot dog model.
