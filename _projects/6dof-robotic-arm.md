---
layout: project

title: "NASA L'SPACE Program"
description: "Led the engineering team through the development of a comprehensive mission design for a hypothetical lunar pit exploration mission focused on investigating permanently shadowed environments and their potential for future human habitation."

start_date: "September 2024"
end_date: "May 2025"

role: "Lead Engineer"

categories: [Project integration, Siemens NX, Leadership, Risk Analysis]
skills:
  - Systems Engineering
  - Mission Design
  - Siemens NX
  - CAD
  - Risk Analysis
  - Project Integration
  - Technical Leadership

categories:
  - Systems Engineering
  - Space Systems
  - CAD
  - Leadership

featured_image: "/assets/images/projects/lspace/lspace_image.jpg"

github_url: ""
demo_url: ""

downloads:
  - name: "Preliminary Design Review"
    file: "/assets/files/lspace/PDR.pdf"
    type: "PDF"

interactive_plot: true

models:
  - file: "/assets/models/robotic-arm/base.gltf"
    description: "Robotic arm base with servo mounting points"
  - file: "/assets/models/robotic-arm/upper-arm.gltf"
    description: "Upper arm segment with gear reduction"

schematics:
  - file: "/assets/schematics/robotic-arm/control-system.svg"
    description: "Main control system with microcontroller and servo drivers"
  - file: "/assets/schematics/robotic-arm/power-distribution.svg"
    description: "Power distribution for servos and control electronics"
  - file: "/assets/schematics/robotic-arm/vision-module.svg"
    description: "Camera module and processing unit connections"


components:
  - name: "Servo Motors (MG996R)"
    quantity: 6
    description: "High-torque digital servo motors for joint actuation"
    link: "https://example.com/mg996r"
    
  - name: "Raspberry Pi 4B"
    quantity: 1
    description: "Main processing unit for computer vision and control"
    link: "https://www.raspberrypi.org/products/raspberry-pi-4-model-b/"
    
  - name: "Arduino Mega 2560"
    quantity: 1
    description: "Servo control and low-level hardware interface"
    
  - name: "PCA9685 Servo Driver"
    quantity: 1
    description: "16-channel PWM servo driver board"
    
  - name: "USB Camera (1080p)"
    quantity: 1
    description: "Computer vision camera with auto-focus"
    
  - name: "3D Printed Parts"
    quantity: 1
    description: "Custom designed arm segments and joints"
    
  - name: "Ball Bearings (608ZZ)"
    quantity: 12
    description: "Smooth rotation for joint mechanisms"
    
  - name: "Power Supply (12V 10A)"
    quantity: 1
    description: "Regulated power supply for servo motors"

gallery:
  - type: "image"
    file: "/assets/images/projects/robotic-arm/featured.jpg"
    description: "6-DOF Robotic arm with vision system"
---
## Overview

I designed and built a six-degree-of-freedom robotic arm...

## Mechanical Design

I designed the arm in SolidWorks...

## Manufacturing

The components were manufactured using...

## Results

The final arm was able to...

files:
  - name: "CAD Assembly"
    file: "/assets/images/carter.jpg"

  - name: "Technical Report"
    file: "/assets/images/carter.jpg"

  - name: "Source Code"
    file: "/assets/images/carter.jpg"
