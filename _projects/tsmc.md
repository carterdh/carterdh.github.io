---
layout: project

title: "TSMC 2026 Summer Internship"
description: "I interned at Taiwan Semiconductor Manufacturing Company (TSMC) over the summer of 2026. I was an equipment engineering intern on the NanoLithography Track. I was responsible for two projects throughout my internship including management responsibilities and technical challenges."

start_date: "June 2026"
end_date: "August 2026"
role: "NanoLithography Equipment Engineer Intern"
skills:
  - Semiconductors
  - Excel VBA
  - Project Management
  - Personnel Management
  - Experiment Design

categories:
  - Semiconductors
  - Management

featured_image: "/assets/images/projects/tsmc/tsmc.jpg"

gallery:
  - type: "image"
    file: "/assets/images/projects/tsmc/tsmc.jpg"
  - type: "image"
    file: "/assets/images/projects/tsmc/proz.jpg"
    description: "The main coater used by Lithography Track team"

---


## Overview

I interned at TSMC Arizona during the summer of 2026 on the Lithography Track team, responsible for one of the highest-throughput processes in the facility. The team operates and maintains the equipment used to apply highly uniform photoresist (PR) coatings to semiconductor wafers.

Track equipment engineers focus on driving nanoscale particle contamination toward zero, maintaining precise coating thickness and uniformity, and continuously monitoring equipment and process data to identify anomalies that could affect wafer quality and yield.

Interns are assigned projects by their department to work on throughout the summer. In my case, I was given two projects, both of which are discussed below.

**DISCLAIMER:** Due to TSMC's Proprietary Information Protection (PIP) policies, I am unable to share many specific details about my projects. As a result, numerical values are presented only as approximate ranges rather than exact figures. I was also unable to retain any documents or materials related to my projects, including the presentation I prepared at the end of the internship. Therefore, the following sections describe my work primarily through narrative explanations rather than specific documentation or data.


## Pump Recycling Project
### Project Overview
One of the common procedures handled by my team was the replacement of coating pumps. Pumps were regularly replaced due to particle contamination or other inconsistencies that could affect wafer quality. Because of the cost and frequency of replacement, I was tasked with determining if pumps could be cleaned after removal from a tool and re-used for production.

I needed to determine **if** a pump could be recycled, **how** to recycle it most efficiently, and **what** impacts the "recyclability of a pump.
### Recyclability Factors
There were multiple factors that I considered to determine the "recyclability" of an individual pump. 

**1. Pump Age**

After a pump is removed from a tool, it is placed in a cabinet before disposal or preparation for a future recycling effort. PR can crystallize while a pump sits idle, so the amount of time a pump has been stored may affect how difficult it is to clean.
  
**2. Photoresist(PR) Properties**

  Different PRs have different properties and are used at different frequencies. The two main properties I considered were viscosity and vapor pressure. Viscosity affects how easily PR may be flushed out, while vapor pressure affects how quickly it may crystallize. Each pump only used one PR in its lifetime, making the PR it was exposed to a potentially important factor in its recyclability.
  
**3. Cleaning Procedure**

Due to proprietary information with the company that makes the pumps, the recycling efforts I was allowed to perform were limited to standard pre-qualification procedures. I had three different procedures I could attempt, which I will refer to as procedures 1, 2, and 3.

### My Actions
The available recycling methods were standard pre-qualification procedures using a qualification tool. Cleaning takes 1-2 weeks, so it was important that I selected the best candidates for recycling and collected data efficiently.

I first determined which PRs were most common and chose candidates based on those properties. I then selected a relatively new pump to establish a baseline and used the most thorough cleaning procedure to determine if recycling was possible.

I repeated this process to collect additional data and compare different pump characteristics and cleaning procedures.

### Outcome
I was only allowed to recycle one pump at a time to leave room on the DPS for production pumps. Since each pump took about two weeks to recycle and I wasn't able to start until later, **three pumps were recycled** over the course of the internship. The criteria to determine if a pump was "clean" was a tool that flushed each pump and recorded particles per mL with a resolution of 18 nanometers. If the average was less than 5 particles/mL, it could considered clean

I was able to successfully determine that pumps could be effectively recycled, but the other questions in my problem statement needed significantly more data to answer reliably. To do that, I needed to create a framework to hand-off to other engineers when I leave.
### Excel VBAs for Project Handover
I made an in-depth Excel file for engineers to use to record progress and analyze data. It included a page to record information on each recycled pump and another page to record available pumps for future recycling. Drawing from that data, I made three Excel macros.
**1. Pump Selection Macro**

This macro was made to tell the engineer which pump to recycle next in order to diversify the data efficiently for analysis. The macro assigned scores to each pump based on characteristics such as age and PR properties. It also considered whether combinations of pump characteristics and cleaning procedures had previously been tested.
**2. Pump Analysis Macro**

This macro took the final data from recycled pumps and generated a recyclability score based on how effectively each pump was recycled. Using this score and the initial pump data, linear regression was used to determine the impact of different factors on pump recyclability.

Because the project required significantly more data before reliable conclusions could be drawn, this analysis was designed primarily as a framework for future engineers to continue developing.
**3. Optimal Pump Selection Macro**

This macro takes the data from the Pump Analysis Macro and the list of available pumps and determines which pump currently available would be the most likely to be recycled effectively.

## DPS Tool Efficiency
### Project Overview
Whenever a new pump is bought, it comes with trace particles that need to be flushed out before production. This process is called "pre-qualification." These processes can be done on main tools, but are mainly done on a dedicated qualification tool. Pre-Q could take upwards of two weeks, slowing production. Much of the additional time came from manually starting recipes, replacing chemical bottles, and coordination between my team and the team operating the qualification tool. My second project was to reduce this gap or at least prove that it could be reduced.
### Actions
For a few weeks, I worked closely with the head of the team to determine areas of inefficiency. The crew was responsible for other tools as well, so I set up remote access to the qualification tool and checked it every few hours, taking screenshots and tracking progress on a Gantt chart.

Working closely with the crew gave me a unique perspective on the difficulties they faced. I tried to give them the benefit of the doubt and treat the disconnect as mainly issues on our side.

They told me they could not obtain enough bottles at a time, so I worked with management to get them a larger cart. They said their bottle supplier was not always available, so I called them and helped rework the schedule. I also clarified a miscommunication between our teams regarding how many bottles they were allowed to obtain each day. Finally, I had daily meetings with the crew's leader to ask about anomalies I noticed and kept the pressure on to make sure the tool remained a priority.

### Outcome
In the end, I was able to reduce pump Pre-Q time by 50%, from two weeks to one week. This made my coworkers very happy!

