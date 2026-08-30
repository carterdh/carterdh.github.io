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

 categories:
   - Mechatronics
   - Mechanical Design

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

For the final of my mechatronics class, our prompt was "make something cool with Arduino that uses sensing, logic, and actuation." I decided to make a center of mass finder with an arm that moves to the center of mass that allows the user to put a sharpie mark at the center. 

On the edges of the plate are four load cells, constantly outputting data based on their deflection. The arm is made up of two stepper motors and simple two linkage inverse kinematics to move the end effector to the correct location on the plate.


## Calibration


## Load Cell Troubleshooting

My biggest challenge in this project was the load cells drifting. The load cells are incredibly sensitive, where even the slightest temperature change can alter their output substantially. I was having a lot of trouble getting consistent results that stayed still. To fix this, I soldered a capacitor across two of the outputs of each load cell to smooth the signal and I implemented a moving average in the code to group outputs together. If I ever redo this project, I would probably replace these with an analog low pass filter.


