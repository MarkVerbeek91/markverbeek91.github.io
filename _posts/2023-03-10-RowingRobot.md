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

# Phases for Reinforced Learning

## Simple mechanics

- Environment with mechanics to convert join angles to position of blade.
- Reward based on distance covered.
- Catching water is simply moving the blade underwater.

## Kinematics

- Environment has notion of speed and total mass of boat+rower.
- Angle joint and torque per joint, results in force
- Penalty for using power.
- Total amount of power available.
- Reward for completing distance with max 2k (or 500 meter)
- Reward for high speed.

## Advanced kinematics

- Mass split into individual parts with own velocity.
  - Boat
  - Lower leg
  - Upper leg
  - Body+head
  - Upper arm
  - Lower arm

## Water interaction

- Blade gets a physical dimension, surface underwater affects efficiency

Note: possible side project for openFOAM. Blade+water interaction.

## Multiple agents (side view)

- assuming sculling boats
- 2 individual agents in a boat (double)
- 4 individual agents in a boat (quad)
- competing boats for evolution

## Multiple agents (top view)

- assuming sweeping boats
- 2 individual agent in a boat (2-)
- 4 individual agent in a boat (4-)
- 8 individual agent in a boat (8+), heavier boat due to cox
- add heading calculation, possible steering
- variation: agent learn from each other

## Simple mechanics in 3D

- Switch to 3D environment
- Mechanics left and right independent (mostly)
- Add joints for shoulders
- Add joints for hip
- heading calculation

## Kinematics in 3D

- same as Kinematics as before

## Advanced kinematics in 3D

- body parts get volume
- body parts can collide

## Water interaction in 3D

- All configurable parameters for rowing in model
  - Oar length, inter/outer
  - rowlock placement and angles
  - Placement of rower in respect to rowlock

## Multiple agents in 3D

- Single sculls competing
- Doubles, pair
- Quad, coxless four
- Eight.
