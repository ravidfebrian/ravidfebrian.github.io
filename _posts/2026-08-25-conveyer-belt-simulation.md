---
title: 'Conveyer Belt Simulation using Codesys and Open Industry Project'
tags:
  - blog
  - Codesys
  - Open Industry Project
---

# Introduction
Industrial automation is everywhere around us—from packaging lines in factories to baggage handling systems at airports—and one of the most common elements in these systems is the conveyor belt. To truly understand how automation works in industries, I decided to create a conveyor belt simulation using Codesys together with resources from the Open Industry Project.

The goal of this project was not only to simulate the movement of a conveyor system but also to practice real-world PLC programming concepts such as sensor integration, motor control, and safety interlocks. By working on this project, I gained hands-on experience with structured programming in Codesys, explored how open-source tools can accelerate learning, and developed a deeper appreciation for the role of simulation in industrial automation.

In this post, I’ll walk you through the setup, the implementation process, the challenges I faced, and what I learned while building this simulation.

# Motivation
Getting started with industrial automation can be challenging, mainly because the hardware and software are expensive. A basic PLC setup with I/O modules, sensors, and actuators can cost hundreds or even thousands of euros, and many industrial software platforms require paid licenses. For student or someone just exploring the field that's nor always realistic.

To overcome this, I looked for tools that are free and open-source but still close to real-world industry standards. Codesys is a software platform for developing and managing industrial automation application using IEC 61131-3 (function block diagram, ladder diagram, structured text, etc.) and it is widely used in industry. On the other hand, the Open Industry Project offers open models and resources that replicate common industrial scenarios, like conveyer systems, in virtual environment.

By combining these two, I was able to simulate a realistic conveyer belt control system, complete with sensors, actuators, and safety logic without needing expensive hardware. This gave me a way to practice  PLC programming, test automation concepts, and debug control logice before moving on to real-world implementations. 

# Project Setup
## Tools
### 1. Development Environment - Codesys 
I used Codesys as my PLC programming environment. It comes with built-in SoftPLC, which allowed me to run the PLC program without real hardware. The logic was written using sturtured text.

### 2. Simulation Model - Open Industry Project 
Open Industry Project is a free and open-source project created by the community to provide open framework to create software and simulations using industrial equipments. This software is based on Godot Engine, which is a free and open-source game engine.

### 3. Communication - OPC UA
OPC UA is a type of industrial communication protocol that enables secure and reliable data exchange between different devices and systems in industrial automation environments. For this project Codesys acts as OPC UA server and Open Industry Project as client. To identify the node Ids from Codesys, I used UaExpert. 

# Implementation

Demos:

<iframe width="560" height="315" 
    src="https://www.youtube.com/embed/gu14V_gtnXc" 
    frameborder="0" 
    allowfullscreen>
</iframe>

<iframe width="560" height="315" 
    src="https://www.youtube.com/embed/b8CdLfw9D2Q" 
    frameborder="0" 
    allowfullscreen>
</iframe>

# Challenges Faced

# Conclussion
- How the architecture looks like. Use draw.io diagram, which are OPC-UA server/client. What is being simulated? (PLC-Sim, Sensors, Actuators, etc.)
- What kind of simulation? Conveyer belt simulation. Include video.
- Challenges. sparse documentation from Open Industry Project for someone who hasn't touch godot like me.
- Conclusion. Know how the industrial communication and sensors in industry. For next, add production line like the one in sorting plant in package delivery. Also, add SCADA monitoring system as a control panel.



