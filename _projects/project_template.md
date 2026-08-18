---
published: false
---

<!--
===============================================================================
                    PROJECT PAGE TEMPLATE / REFERENCE
===============================================================================

This file is ONLY a reference.

DO NOT uncomment everything at once.

Copy the sections you actually need into a new project .md file.

The only active YAML above is:

    published: false

That prevents this reference file from appearing on the website.

===============================================================================
                              QUICK STRUCTURE
===============================================================================

A normal project file should look roughly like:

    ---
    layout: project

    title: "My Project"
    description: "Short description."

    start_date: "January 2025"
    end_date: "May 2025"
    role: "Mechanical Designer"

    skills:
      - SolidWorks
      - CAD
      - 3D Printing

    categories:
      - Robotics
      - Mechanical Design

    featured_image: "/assets/images/projects/my-project/featured.jpg"

    downloads:
      - name: "CAD Assembly"
        file: "/assets/files/my-project/assembly.step"
        type: "CAD"

    models:
      - file: "/assets/models/my-project/model.glb"
        description: "Complete assembly"

    gallery:
      - type: "image"
        file: "/assets/images/projects/my-project/photo.jpg"
        description: "Project photo"

    schematics:
      - file: "/assets/schematics/my-project/circuit.svg"
        description: "Main circuit schematic"

    ---

    ## Project Overview

    Write the actual project description here.

===============================================================================
                          1. BASIC PROJECT INFORMATION
===============================================================================

These are the basic fields that control the project title and information
shown on the LEFT side of the project page.

Copy whichever ones you need.
-->

<!--

---
layout: project

title: "Project Title"

description: "Short one- or two-sentence description of the project."

# Project timeline
start_date: "January 2025"
end_date: "May 2025"

# Your role in the project
role: "Lead Mechanical Engineer"

# Skills / technologies used
skills:
  - Mechanical Design
  - CAD
  - SolidWorks
  - Siemens NX
  - Arduino
  - C++
  - 3D Printing
  - Electronics

# Categories / broad project topics
categories:
  - Robotics
  - Mechanical Design
  - Embedded Systems

# Main image used to represent the project elsewhere on the site
featured_image: "/assets/images/projects/your-project/featured.jpg"

# Optional external links
github_url: "https://github.com/username/project"
demo_url: "https://example.com"

---

-->

<!--
===============================================================================
                              2. DOWNLOADS
===============================================================================

This creates the "Downloads" section on the LEFT side.

Use this for files you want visitors to download.

Examples:
- STEP files
- STL files
- PDFs
- CAD drawings
- source code
- ZIP files
- reports
- BOMs
- spreadsheets
- anything else

The "type" controls the icon shown next to the file.

Common types:
    CAD
    STEP
    STL
    Code
    PDF
    Drawing

Anything else gets a generic file icon.
-->

<!--

downloads:

  - name: "Complete CAD Assembly"
    file: "/assets/files/your-project/assembly.step"
    type: "CAD"

  - name: "3D Printable Parts"
    file: "/assets/files/your-project/parts.zip"
    type: "STL"

  - name: "Project Report"
    file: "/assets/files/your-project/report.pdf"
    type: "PDF"

  - name: "Engineering Drawing"
    file: "/assets/files/your-project/drawing.pdf"
    type: "Drawing"

  - name: "Arduino Firmware"
    file: "/assets/files/your-project/main.ino"
    type: "Code"

-->

<!--
===============================================================================
                            3. 3D MODEL FILES
===============================================================================

These appear on the RIGHT side using the interactive 3D model viewer.

Supported model formats from the original template include:

    STL
    OBJ
    GLTF
    GLB

The model is displayed interactively with camera controls.

IMPORTANT:
The current layout renders ALL models together before the gallery.

So:

    models:
      - model A
      - model B

will produce:

    MODEL A
    MODEL B

before the gallery starts.

If you later change the layout to a unified media system, this may change.
-->

<!--

models:

  - file: "/assets/models/your-project/main-assembly.glb"
    description: "Complete project assembly"

  - file: "/assets/models/your-project/chassis.glb"
    description: "Robot chassis"

  - file: "/assets/models/your-project/arm.glb"
    description: "Robotic arm assembly"

-->

<!--
===============================================================================
                             4. IMAGE / VIDEO GALLERY
===============================================================================

These appear on the RIGHT side below the 3D models.

The gallery supports:

    JPG
    JPEG
    PNG
    GIF
    WebP

It also supports video files:

    MP4
    WebM
    AVI

The layout automatically detects video files by their extension.

Each gallery item can have a description/caption.

The order here determines the order of the gallery items.
-->

<!--

gallery:

  # Regular image
  - type: "image"
    file: "/assets/images/projects/your-project/front.jpg"
    description: "Front view of the completed assembly"

  # Another image
  - type: "image"
    file: "/assets/images/projects/your-project/testing.jpg"
    description: "System during testing"

  # Animated GIF
  - type: "image"
    file: "/assets/images/projects/your-project/demo.gif"
    description: "Demonstration of the mechanism"

  # Video
  - type: "video"
    file: "/assets/images/projects/your-project/demo.mp4"
    description: "Full system demonstration"

  # Another video
  - type: "video"
    file: "/assets/images/projects/your-project/assembly.mp4"
    description: "Assembly process"

-->

<!--
===============================================================================
                              5. SCHEMATICS
===============================================================================

These appear on the RIGHT side below the other media.

The current layout displays schematic files as images.

Supported examples:

    PNG
    JPG
    SVG
    PDF

NOTE:
The current layout uses an <img> element, so SVG/PNG/JPG are the safest
choices for something you want displayed directly.

If you want a PDF to be downloadable rather than displayed, put it under
"downloads" instead.
-->

<!--

schematics:

  - file: "/assets/schematics/your-project/main-circuit.svg"
    description: "Main circuit schematic"

  - file: "/assets/schematics/your-project/power.svg"
    description: "Power distribution schematic"

  - file: "/assets/schematics/your-project/sensor.svg"
    description: "Sensor wiring schematic"

-->

<!--
===============================================================================
                         6. COMPONENTS & MATERIALS
===============================================================================

This creates a Components & Materials table on the LEFT side.

Each component can have:

    name
    quantity
    description
    link

IMPORTANT:
The current project layout displays the NAME and QUANTITY.

The description/link fields are part of the original project data structure,
but the current layout does not display them in the table.

Example:
-->

<!--

components:

  - name: "Arduino Uno"
    quantity: 1
    description: "Main microcontroller"
    link: "https://store.arduino.cc/products/arduino-uno-rev3"

  - name: "NEMA 17 Stepper Motor"
    quantity: 2
    description: "Drive motors"
    link: ""

  - name: "608ZZ Bearing"
    quantity: 8
    description: "Rotational support bearings"
    link: ""

-->

<!--
===============================================================================
                              7. CODE FILES
===============================================================================

This is the ORIGINAL code system from the MESGRO template.

It can do two things:

1. Provide a downloadable link to code.
2. Display the actual code inside a collapsible code viewer.

You probably won't need "content" for most future projects.

For your portfolio, I recommend using the simpler DOWNLOADS system instead
if you just want people to download code.

Use code_files when you specifically want the code displayed on the page.
-->

<!--

code_files:

  - name: "Main Arduino Firmware"
    file: "main.ino"
    language: "cpp"
    download_url: "https://github.com/username/project/blob/main/main.ino"

  - name: "PID Controller"
    file: "pid_controller.py"
    language: "python"
    download_url: "https://github.com/username/project/blob/main/pid_controller.py"

-->

<!--
===============================================================================
                    8. CODE FILES WITH EMBEDDED CONTENT
===============================================================================

You can also put the actual source code directly into the Markdown file.

I DO NOT recommend doing this unless you specifically want visitors to be
able to expand and read the code directly on your project page.

This can make project files extremely large.

Example:
-->

<!--

code_files:

  - name: "Main Arduino Firmware"
    file: "main.ino"
    language: "cpp"
    download_url: "https://github.com/username/project/blob/main/main.ino"

    content: |
      #include <Arduino.h>

      void setup() {
          Serial.begin(115200);
      }

      void loop() {
          // Main control loop
      }

-->

<!--
===============================================================================
                           9. DATA VISUALIZATIONS
===============================================================================

The "visualizations" system embeds a file inside an iframe on the RIGHT side.

This is useful for:
    - HTML plots
    - dashboards
    - custom interactive visualizations
    - standalone visualization pages

Each item has:

    file
    description
-->

<!--

visualizations:

  - file: "/assets/data/plots/temperature.html"
    description: "Temperature over time"

  - file: "/assets/data/plots/pressure.html"
    description: "Pressure during testing"

-->

<!--
===============================================================================
                       10. INTERACTIVE CSV PLOTS
===============================================================================

Your site also supports the interactive Plotly CSV system.

Enable it with:

    interactive_plot: true

Then provide the appropriate plot configuration.

===============================================================================
                           SIMPLE PLOT
===============================================================================

Use this for one X dataset and one Y dataset.
-->

<!--

interactive_plot: true

plot_config:
  title: "Temperature Over Time"

  x_file: "/assets/data/plots/time_data.csv"
  y_file: "/assets/data/plots/temperature_data.csv"

  x_label: "Time (seconds)"
  y_label: "Temperature (°C)"

-->

<!--
===============================================================================
                         MULTI-DATASET PLOTS
===============================================================================

The "plots" system can use different columns from CSV files.

This is useful for things like:

    time vs temperature
    time vs humidity
    time vs pressure

all on one visualization.
-->

<!--

interactive_plot: true

plots:

  - title: "Environmental Conditions"

    x_file: "/assets/data/plots/sensor_data.csv"
    x_column: 0
    x_label: "Time (minutes)"

    y_files:

      - file: "/assets/data/plots/sensor_data.csv"
        column: 1
        label: "Temperature (°C)"

      - file: "/assets/data/plots/sensor_data.csv"
        column: 2
        label: "Humidity (%)"

      - file: "/assets/data/plots/sensor_data.csv"
        column: 3
        label: "Pressure (hPa)"

-->

<!--
===============================================================================
                              11. CUSTOM PLOTS
===============================================================================

The layout also supports a custom Liquid include.

Set:

    custom_plot: "filename.html"

The layout will load that file from _includes/.

Example:
-->

<!--

custom_plot: "my-custom-plot.html"

-->

<!--
===============================================================================
                         12. MARKDOWN CONTENT
===============================================================================

Everything AFTER the closing "---" in a normal project file becomes the
written project content.

This is where you write the actual story of the project.

Use normal Markdown.

Suggested structure:
-->

<!--

## Project Overview

Explain:

- What you built
- Why you built it
- What problem it solves
- What your contribution was

## Design

Explain the engineering design.

### Mechanical Design

Describe the mechanical system.

### Electrical Design

Describe the electronics.

### Software

Describe the firmware/software.

## Testing & Results

Describe how you tested the system and what happened.

### Performance

Include measured results.

| Metric | Result |
|---|---:|
| Maximum Speed | 1.2 m/s |
| Accuracy | 95% |
| Battery Life | 45 min |

## Challenges

Describe the major engineering problems you encountered.

## Solutions

Explain how you solved them.

## Lessons Learned

Explain what you learned.

## Future Improvements

Explain what you would change in another version.

-->

<!--
===============================================================================
                         13. MARKDOWN FEATURES
===============================================================================

Normal Markdown supports:

HEADINGS
-->

<!--

# Heading 1

## Heading 2

### Heading 3

-->

<!--
PARAGRAPHS
-->

<!--

This is a normal paragraph.

You can write multiple paragraphs.

-->

<!--
BOLD / ITALICS
-->

<!--

**Bold text**

*Italic text*

**Bold and *italic* text**

-->

<!--
BULLET LISTS
-->

<!--

- Item one
- Item two
- Item three

-->

<!--
NUMBERED LISTS
-->

<!--

1. First step
2. Second step
3. Third step

-->

<!--
LINKS
-->

<!--

[GitHub Repository](https://github.com/username/project)

-->

<!--
IMAGES IN THE WRITTEN DESCRIPTION
-->

<!--

![Description](/assets/images/projects/your-project/design.jpg)

-->

<!--
CODE BLOCKS
-->

<!--

```cpp
void setup() {
    Serial.begin(115200);
}
