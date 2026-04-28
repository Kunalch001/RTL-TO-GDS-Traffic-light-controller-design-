# RTL-to-GDS Design of 4-Way Traffic Light Controller

## Project Overview

This project implements a 4-way traffic light controller using the RTL-to-GDS flow in VLSI design. The controller manages traffic at a four-road intersection by controlling Red, Yellow, and Green signals for each direction.

The design is based on two traffic variables for every direction:

* Straight movement signal
* Right-turn movement signal

Left-turn movement is considered a don’t-care condition in the control logic.

The project demonstrates the complete design cycle from RTL coding to physical layout generation using standard VLSI design methodology.

---

## Objective

The main objective of this project is to design and implement a traffic signal controller that automates signal switching for a 4-way intersection while following the complete RTL-to-GDS design flow.

---

## Features

* 4-way traffic signal control
* Finite State Machine (FSM)-based design
* Separate handling for straight and right-turn movement
* Left-turn considered as don’t-care logic
* RTL coding and functional simulation
* Gate-level synthesis
* Physical design implementation
* Final GDSII layout generation

---

## Design Flow

The project follows the standard RTL-to-GDS flow in VLSI:

1. RTL Design using Verilog/VHDL
2. Functional Simulation
3. Logic Synthesis
4. Floorplanning
5. Placement
6. Clock Tree Synthesis (CTS)
7. Routing
8. DRC/LVS Verification
9. GDSII Generation

---

## Inputs

* Clock Signal
* Reset Signal
* Traffic timing control
* Straight movement request
* Right-turn movement request

## Outputs

* Red Signal
* Yellow Signal
* Green Signal

for all four directions.

---

## Working Principle

The controller operates sequentially using FSM logic.

Example sequence:

1. North-South Green, East-West Red
2. North-South Yellow, East-West Red
3. East-West Green, North-South Red
4. East-West Yellow, North-South Red

The sequence repeats continuously based on clock timing.

---

## Tools Used

* Verilog HDL / VHDL
* Xilinx Vivado / ModelSim / Cadence Tools
* Synopsys Design Compiler
* Physical Design Tools for Layout Generation

---

## Applications

* Smart traffic management systems
* Automated road intersections
* Urban traffic control systems
* Intelligent transportation systems

---

## Conclusion

This project successfully demonstrates the RTL-to-GDS design methodology by implementing a 4-way traffic light controller. It provides practical knowledge of digital design, FSM implementation, synthesis, and physical design stages in VLSI.
