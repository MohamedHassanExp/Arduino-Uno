# Arduino Uno Custom Hardware Design

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)
[![KiCad](https://img.shields.io/badge/KiCad-FFFFFF?style=flat-square&logo=kicad&logoColor=blue)](https://www.kicad.org/)
[![Arduino](https://img.shields.io/badge/-Arduino-00979D?style=flat-square&logo=Arduino&logoColor=white)](https://www.arduino.cc/)

A custom-designed printed circuit board (PCB) based on the Arduino Uno architecture, featuring full schematic capture, layout, and manufacturing-ready fabrication files.

##  Table of Contents
- [About the Project](#about-the-project)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Repository Structure](#repository-structure)


##  About the Project

This project contains the complete hardware design files for an Arduino Uno development board. It serves as a physical hardware platform for embedded C/C++ programming, prototyping, and peripheral integration.

### Tech Stack
*   **EDA Software:** KiCad (for schematic capture and PCB layout)
*   **Hardware Target:** Arduino Uno

##  Getting Started

Follow these instructions to view or modify the hardware design files locally.

### Prerequisites

*   [KiCad EDA](https://www.kicad.org/download/) to open the core project files.
*   A standard Gerber viewer (if you only want to inspect the manufacturing layers).

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/MohamedHassanExp/Arduino-Uno.git
2. Navigate to the project directory
   ```bash
   cd Arduino-Uno-main
3. Open `Arduino uno.kicad_pro` project file using KiCad.

## Repository Structure

The repository is organized to separate the editable design files from the static manufacturing outputs:

*   **Design Files:**
     The root directory contains the core KiCad project files, including the schematic (Arduino uno.kicad_sch) and the physical layout (Arduino uno.kicad_pcb).
*    **Board Renders:**
      High-resolution 3D renders of the physical layout are available as Arduino uno-front.png and Arduino uno-back.png.  
*    **Manufacturing Files (/Manufacturing/):** 
      This directory contains everything a fabrication house like JLCPCB or PCBWay needs to manufacture and assemble the board:
      * **Arduino uno-gerber.rar:** The compressed Gerber layers and drill files for PCB fabrication.
      * **Arduino uno-BOM.csv:** The complete Bill of Materials for component sourcing and assembly.
      * **Arduino uno-position.csv:** The centroid/pick-and-place data for automated SMD assembly.
