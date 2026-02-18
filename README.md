# Synchronous FIFO Design (Verilog/SystemVerilog)

## Project Overview

This project implements a parameterizable Synchronous FIFO (First-In-First-Out) memory using Verilog/SystemVerilog. The design supports configurable data width and depth and includes status flags such as full and empty. A self-checking testbench is provided to verify functionality through simulation.

---

## Design Features

- Synchronous FIFO architecture (single clock domain)
- Parameterizable DATA_WIDTH and DEPTH
- Full and Empty flag generation
- Write and Read pointer management
- Overflow and Underflow protection
- Synthesizable RTL design
- Clean and modular coding style

---

## FIFO Architecture

The design consists of:

- Memory array for data storage
- Write pointer
- Read pointer
- Full flag logic
- Empty flag logic

Operation:
- On write enable and not full, data is written and write pointer increments
- On read enable and not empty, data is read and read pointer increments

---

## Simulation Details

- Simulator Used: EDA Playground
- Language: SystemVerilog (IEEE 1800)
- Waveform Viewer: EPWave / GTKWave
- Testbench verifies:
  - Normal write and read operations
  - FIFO full condition
  - FIFO empty condition
  - Overflow attempt
  - Underflow attempt

---

## Directory Structure
FIFO/
│── rtl/
│ └── fifo.sv
│── tb/
│ └── fifo_tb.sv
│── sim/
│ └── waveform.png



 
---

## How to Run

1. Copy RTL and Testbench code into EDA Playground
2. Select SystemVerilog (IEEE 1800)
3. Choose any supported simulator (e.g., Questa, Aldec, etc.)
4. Run the simulation
5. Open EPWave to view signals

---

## Key Learning Outcomes

- Understanding FIFO architecture and memory design
- Pointer arithmetic and wrap-around logic
- Full and Empty flag generation techniques
- Writing structured and synthesizable RTL
- Developing verification-oriented testbenches

---

## Author
Meghana Bollu
Electronics and Communication Engineering Graduate
Aspiring Design Verification Engineer



