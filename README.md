🚧 PLC Conveyor Belt Metal Detector System

Course: Programmable Logic Controllers (PLC216D)
Department: Computer Systems Engineering
Institution: Tshwane University of Technology
Semester: 2, 2025
Lecturer: Mr. I.L. Machele
Date: 30 October 2025

🧭 Project Overview

This project was developed as part of the GA Practical Experiment for the PLC216D course.
The objective was to design and implement a recycling plant conveyor system that automatically sorts mixed materials (metallic and non-metallic) using a bidirectional conveyor belt and a metal detection sensor.

The system detects metallic objects and reverses the conveyor belt so that these objects are placed in a separate container from the non-metallic materials. The project also includes Start and Emergency Stop functionality for safe operation.

🎯 Aim and Objectives

Detect metallic components in the mix using a proximity sensor.

Automatically change the conveyor belt direction based on object type:

Forward for non-matellic materials

Reverse for metallic materials

Separate materials into two containers.

Implement functional Start and Emergency Stop buttons.

⚙️ System Components
Component	Description
PLC Software	Siemens TIA Portal V12
PLC	Siemens PLC (current sourcing configuration)
Sensor Type	NPN Inductive Proximity Sensor (3-wire)
Power Supply	24V DC stepped down to 5V DC for breadboard circuits
Actuators	Bidirectional DC Motor (for conveyor control)
Indicators	Red LED (metal detected), Green LED (no metal detected)
Control Buttons	Start and Stop push buttons

🧠 Working Principle

The conveyor belt moves forward to transport mixed materials.

The NPN proximity sensor detects metallic objects by creating a path to ground when triggered.

The PLC receives the signal and:

Stops and reverses the conveyor direction for metal objects.

Activates the Red LED indicator.

For other objects, the belt continues moving forward and activates the Green LED.

The system can be started with the Start button and halted immediately with the Stop button.

🪜 Ladder Logic Development

The ladder diagram was first designed and simulated using the PLC Fiddle online tool due to limited access to TIA Portal outside the lab.

The component addresses in the simulation were aligned closely with the actual PLC hardware addresses to ensure smooth transfer and testing during lab sessions.

Final testing and program download were done using TIA Portal V12 once in the lab.

🧩 Hardware Setup Notes

The NPN sensor’s wiring was configured as follows:

Brown → L+ (24V)

Black → PLC input (signal)

Blue → Left unconnected (acts as ground when triggered)

The sensor was mounted above the conveyor belt to detect metals efficiently without contact.

The original conveyor belt motor was replaced with a provided bidirectional motor for control testing.

👥 Team Roles and Responsibilities

The project was completed by a group of 5 students with clearly defined roles:

Role	Responsibility
2 Members	Documentation, troubleshooting, and system report preparation
1 Member	Built the conveyor belt structure, ensured mechanical stability, and proper sensor placement relative to the conveyor
2 Members (including myself)	Developed and tested the ladder logic, configured inputs/outputs, downloaded the program to the PLC, and verified full system operation

🔍 Reflections

This project strengthened our understanding of:

Sensor interfacing with PLCs (sinking/sourcing configurations)

Safe wiring practices for automation systems

Practical application of ladder logic for industrial control

Team collaboration in both hardware and software aspects

🏷️ Tags
#PLC #Automation #TIA_Portal #Engineering #StudentProjects #IndustrialControl

Author: Tsietsi Mahasa (and Group Members)
Course: PLC216D — Department of Computer Systems Engineering
Date: October 2025
