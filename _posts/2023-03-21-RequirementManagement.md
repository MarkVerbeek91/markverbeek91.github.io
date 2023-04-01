---
title: Requirement Engineering
author: Mark Verbeek
layout: post
date: 2023-03-23 08:30:00 +/-0800
categories: [Programming, Requirements]
tags: [engineering, management, tooling, planning]
pin: false
mermaid: true
---

> Work in progress (use at own risk):
{: .prompt-tip }

# Requirement Management

In the domain of engineering, independent of type, requirements are the driving force of any project [citation needed].

Without requirements there is nothing to engineer. The field of requirement engineering will be on of the starting ground tot start a project [again, citation needed]

Any projects will start with a wish, a vision or desire [I guess, I need again a citation]. Without this wish, wonder of desire there is nothing to improve on the current situation.

From this wish, vision or desire there will be requirements, and usually it will end up with a lot of requirements. This is the field of requirement engineering.

## after requirements come?

So the project starts with a vision, wish or desired of what the project should do. This is usually very high level. For example:

- I want to build a tree hut
- Eliminate world hunger
- I want to build a rowing robot
- My wife wants a clean house

For simplicity, we shall call these visions for the remainder of the text.

Each of these visions can be (and should be) broken down in smaller pieces. Each of these piece will be a requirement to shape the vision. Without them, it would be anyone guess when the vision shall be completed. Without this breakdown a tree hut could be made out of a soft material instead of solid one.

- The tree hut shall be able to hold up to 3 children of age 10.

The next step is to determine a method to fulfill the requirement. This is done by a design decision (DD).

- It's decided that the tree hut shall be made out of wood.

From this DD more requirement can come, or a DD can fulfill multiple requirements. Like for this example that the tree hut would be cheap and/or easy to build.

Keeping track of requirements and design decision can be done by requirement management, this can be a post-it on the wall with wire connecting them. This would like work for very small projects. For most, and rapid changing projects this would not work. So we need a tool

## Requirement management tool

TODO:

[] create a list of available tools
[] compare the tools
[] see if still make sense to explore own solution
[] add conclusion

## When proceeding with implementation

- can use NiceGUI to 100% implement in python, local app
- Javascript frond end, django backend (standard approach)

## Process of creating a Product Specification

- start with the goal. What is the wish, and what is the rationale for this wish.

  - I want a tree hut, because I want to play outside.

- Then list the requirements

  - The tree hut shall have a floor
  - The tree hut shall have a roof
  - The tree hut shall be place in a tree
  - The tree hut shall be placed 2 meters above the ground
  - etc.

- Each of these requirements can be either be broken down in to more requirements or to a design decision.

  - The tree hut shall have a floor
     - The floor shall be able to hold 3 children, aka 150 kg.
     - The floor shall be made of a cheap material, max €50

  - The tree hut shall be place in a tree
    - It is decided that the tree hut is build in the tree in the back garden.
    - Rationale: this object is a tree, and it's close by.

From there the tree (no pun intended) for requirements goes on. Breaking down each object till each requirement has a design decision.
