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
  - file: "/assets/files/loop/suspension_assem.glb"
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

UMD Loop is a student team that competes in the University Rover Challenge. I was on the suspension sub-team, so my job was to design everything between the chassis and the wheels. In the 2025 season, we were designing a material dampener system to distribute loads across the rover and help it survive extreme drops. Unfortunately, due to weight concerns this dampener system was scrapped in favor of swerve steering modules.

## Design

The biggest challenge of this design was optimizing the dimensions and elastic modulus of the material dampener to compress to the desired size when under a static load and properly distribute the load when under a dynamic/shock load. To preform this optimization, I first solved the system statically to reveal the relationships between the normal force applied on the wheels and the lever-arm compression of the foam. Through this process and with consultation with a professor, I realized that the system had far too many variables to solve by hand, so I decided so set up an FEA and test multiple materials to test how they would work in various environments. Multiple materials were chosen as candidates and a mounting system was in preliminary design phases when we were informed the system would be sacrificed.

## Outcome

Although the material dampener was scrapped, the suspension itself still needed to be present to support the chassis and the differential bar. Reverting to (and slightly altering) an earlier design was the agreed upon solution. Parts were ordered from McMaster Carr and bent sheet metal parts were ordered from SendCutSend. The linkages were cut to size and the suspension was assembled and mounted by me for the final competition.



