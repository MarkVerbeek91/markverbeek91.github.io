---
title: Rowing Robot
author: Mark Vebreek
date: 2023-03-10 08:30:00 +/-0800
categories: [Robotics, Programming]
tags: [robot, embedded, python, rust, c++/c]
pin: true
mermaid: true
---

# Rowing Robot

Can a robot row? most cannot and most robot sink, too.

Can we teach a robot to row? yes, very likely, lets find out:

Why teach a robot to row? it's fun, and we might learn a thing or two. About building robots for me personal, but perhaps also about rowing itself.

Should a robot row? no, but it's fun, at the moment of writing this.

This project is, at the moment, a project for me to explore new subjects, software or other various concepts. So some components might feel like overkill for the above goal, there here because I thought it was fun.

# Getting started:

To have a robot rowing in a boat we need to split to challenge in multiple parts.

We can make the split in hardware and software.

The hardware we split into the boat and to robot. The end goal is to build a robot to row in a real boat. Since very high goal, we first start small.

So at some point we need a miniature boat.

# Project Components

Robotics is a mix of hardware, electronics and software [citation needed]. With all these three components I want to take a more or less software approach. This means I have simulation and testing for the hardware and electronic designs, just like for the software components.

## Hardware Components

Overview of involved hardware components:

### The robot

Collections of parts, motors, electronics and power source.

### The boat

Assembly of a hull, riggers, ors, etc.

OpenFOAM can be used to simulator the behaviour of the board and blades in the water.

### Test rig

Of course, we need to test.

## Software components

Overview of involved software components

### Robot brain

Controller for the robot, like running on some embedded board.

### Machine Learning

For the robot brain to know how to row, it needs to be trained.

Another option is to derive a motion based on first principles. This can be done, and might be a valid solution. A comparison could be made here.

### Hardware testing (simulation, digital twin)

(unit) test the hardware, coalition detection and FEM for rigidity testing.

### Electronic testing (simulation)

(unit) testing the electronics. Pulse propagation, etc

Use of KiCAD and QEMU.

## Electronics

Overview of electronics

### CPU

Hardware board selections, STM series?

### PCB

Controller board

### Electric plan

Assembly of all PCBs, motors, sensors and wires.

# Future plans, and etc

## Draft notes, possible chapters

- 1:10 scale.
- FreeCAD
- KiCAD
- Digital Twin
- OpenFOAM
- Blender Renders
- MachineLearning (Reinforced Learning)
