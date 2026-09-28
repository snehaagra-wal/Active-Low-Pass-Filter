# Active Low-Pass Filter Design (KiCad)
<img width="963" height="1280" alt="WhatsApp Image 2026-09-28 at 17 52 28" src="https://github.com/user-attachments/assets/f62edaf7-33bb-4060-a530-f34d9dafef32" />


## Overview
This project features a complete hardware design for an **Active Low-Pass Filter** developed using **KiCad**. The project includes the complete schematic capture, PCB layout, 3D visualization, and manufacturing-ready Gerber files. 

*Note: KiCad is a powerful Electronic Design Automation (EDA) software used for schematic capture and PCB layout. It functions as a digital design and modeling tool, allowing engineers to create precise blueprints, virtual 3D models, and fabrication files (Gerbers) to visualize and verify how a physical circuit board will be constructed prior to manufacturing.*

---

## What Does This Circuit Do?
An active low-pass filter allows signals with a frequency lower than a specific cutoff frequency to pass while attenuating signals with frequencies higher than the cutoff. By incorporating an active component (an operational amplifier), this circuit provides signal amplification and prevents loading effects, ensuring stable and reliable performance for analog signal processing applications.

---

## Circuit Architecture & Component Connections
The circuit design is structured around a dual operational amplifier setup and passive filtering elements:
* **Resistors (R1, R2):** Positioned in the signal path to set the filter's characteristics and frequency response.
* **Capacitors (C1, C2):** Connected in conjunction with the resistors to establish the RC time constants that determine the cutoff frequency.
* **Operational Amplifier (U1A - Opamp_Dual):** Configured to buffer and amplify the filtered signal, providing high input impedance and low output impedance.
* **Ground Plane (GND):** A full copper pour (ground plane) has been integrated into the PCB layout to minimize electromagnetic interference (EMI), reduce noise, and provide a stable reference voltage across the board.

---

## Design & Manufacturing Workflow (KiCad)
1. **Schematic Capture:** Designed the logical electronic circuit using KiCad's schematic editor (`.kicad_sch`), mapping out all components, nets, and power connections.
2. **PCB Layout & Copper Pour:** Routed the traces and implemented a full copper ground plane on the PCB (`.kicad_pcb`) to ensure signal integrity.
3. **3D Visualization:** Utilized KiCad's built-in 3D Viewer to inspect the virtual board, component placement, and clearance before fabrication.
4. **Gerber & Drill Generation:** Exported standard manufacturing files (Gerbers and `.drl` drill files) ready for physical production.

---

## Manufacturing Options
While this repository contains the complete design files for simulation and fabrication review, physical manufacturing can be carried out using industry-standard PCB fabrication houses such as:
* **JLCPCB**
* **PCBWay**

Simply upload the generated Gerber and drill zip folder to either platform to get physical prototypes made.
