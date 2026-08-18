---
layout: project
title: "UMD Loop Suspension"
description: "I was a part of UMD Loop, a student team competing in the University Rover Challenge, where we design and build a rover capable of tackling complex mobility and scientific tasks. My role was on the suspension sub-team, where I focused on designing and refining the rover’s two-arm suspension system."
start_date: "September 2024"
end_date: "May 2026"
categories: [SolidWorks, DFM, Manufacturing]
skills:
  - SolidWorks
  - Project Integration
  - FEA Simulation
  - Teamwork
  - COTS Design
  - Metalworking

featured_image: "/assets/images/projects/loop/loop1.jpg"

models:
  - file: "/assets/files/loop/suspension assem.STL"
    description: "Early suspension CAD"


gallery:
  - type: "image"
    file: "/assets/images/projects/loop/loop1.jpg"
    description: "Internals of free joint to allow for smooth movement"
  - type: "image"
    file: "/assets/images/projects/loop/loop2.jpg"
    description: "Conceptual material dampener representation"
---

## Overview

UMD Loop is a student team that competes in the University Rover Challenge. I am on the suspension sub-team, so my job is to design everything between the chassis and the wheels. In the 2025 season, we are designing a material dampener system to distribute loads across the rover and help it survive extreme drops.

## Design
The biggest challenge of this design was optimizing the dimensions and elastic modulus of the material dampener to compress to the desired size when under a static load and properly distribute the load when under a dynamic/shock load. To preform this optimization, I first solved the system statically to reveal the relationships between the normal force applied on the wheels and the lever-arm compression of the foam. I then wrote a MATLAB script to optimize the dimensions of the foam in order to compress to the desired angular dimensions that give us the required wheelbase and ride height. It gives me a series of combinations of dimensions paired with a calculated elastic modulus. I was then able to match the calculated elastic moduli to real datasheets and choose the correct dampener. 



