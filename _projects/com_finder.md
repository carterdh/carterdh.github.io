---
 layout: project

 title: "Center of Mass Finder"
 description: "For the final project of my mechatronics class, I made a center of mass finder with an arm that points to the center of mass of an object placed on the plate."

 start_date: "March 2026"
 end_date: "May 2026"

 skills:
   - SolidWorks
   - CAD
   - 3D Printing
   - Actuation
   - Load cells
   - Signal processing
   - Arduino

 categories:
   - Mechatronics
   - Mechanical Design
   - Arduino

 featured_image: "/assets/images/projects/com/com1.jpeg"

 downloads:
   - name: "CAD Assembly"
     file: "/assets/files/com/COM Finder CAD.zip"
     type: "zip"
   - name: "Calibration Code Arduino"
     file: "/assets/files/com/Lab 9 Calibration Arduino.pdf"
     type: "pdf"
   - name: "Calibration Code Matlab"
     file: "/assets/files/com/Lab 9 Calibration Matlab.pdf"
     type: "pdf"
   - name: "Main Arduino Code"
     file: "/assets/files/com/Lab 9 Main Arduino.pdf"
     type: "pdf"
   - name: "Processing Code"
     file: "/assets/files/com/Lab 9 Processing.pdf"
     type: "pdf"

 models:
   - file: "/assets/files/com/full_assem.glb"
     description: "Complete assembly"

 gallery:
   - type: "youtube"
     file: https://www.youtube.com/watch?v=iR6r2DKwyKw
     description: "Submission Video"
   - file: "/assets/images/projects/com/com2.jpeg"

    
---
## Overview

For the final of my mechatronics class, our prompt was "make something interesting with Arduino that uses sensing, logic, and actuation." I decided to make a center of mass finder with an arm that moves to the center of mass that allows the user to put a sharpie mark at the center. 

On the edges of the 200x200mm plate are four load cells, constantly outputting data based on their deflection. The arm is made up of two stepper motors and simple two linkage inverse kinematics to move the end effector to the correct location on the plate.


## Calibration

Since the load cells only output 24 bit ADC values, calibration must be done to determine how each load cell's values match up to specific weights or weight distributions. This calibration needed to be done  while also considering the significant drift the load cells were producing (see the "Load Cell Troubleshooting" section). 

I wrote a MATLAB script where I could input known data and get a calibration matrix. The MATLAB script calibrates the four load cells by using several measurements with a known 200 g weight placed at known x and y coordinates on the plate. It solves a linear system to find a 3×4 calibration matrix that converts the four raw sensor readings into total weight W, Wx, and Wy. The COM coordinates are then calculated as x = Wx / W and y = Wy / W. The script outputs the calibration matrix in C/C++ format for use on the microcontroller, along with the condition number and estimated weight/COM for each calibration point to verify the accuracy of the calibration.

## Load Cell Troubleshooting

My biggest challenge in this project was the load cells drifting. The load cells are incredibly sensitive, where even the slightest temperature change can alter their output substantially due to thermal expansion. I was having a lot of trouble getting consistent results that stayed still. To fix this, I soldered a capacitor across two of the outputs of each load cell to smooth the signal and I implemented a moving average in the code to group outputs together. If I ever redo this project, I would probably replace these with an analog low pass filter.

## Actuation

I decided to create a two linkage revolute joint arm to move the end effector to the calculated center of mass. I used a NEMA 17 for the inner joint and a lighter/smaller stepper motor for the outer joint. I designed the 3d printed arm to be as light as possible to minimize skipping. 

Both motors needed a "home" position to begin each process so that there is some reference. To implement this with as few moving parts as possible, I made a sort of docking system where I would physically move the arm until a tab on the arm was fully enclosed by a slot near the motor mount.

To calculate the positioning, I used the standard two linkage inverse kinematics formulas. I extracted the angle data from the amount of steps moved by each motor and extracted the linkage length information from the CAD. 

## Outcome and Reflection

This project was able to consistently position the end effector within ~2mm of the actual location of the center of mass, which I consider a success! I had never worked with load cells before and was able to learn a lot from this process. If I were to redo this project, I would pay greater attention to 

