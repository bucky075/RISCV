# 64-bit RISC-V 5-stage Pipeline

This project implements a simplified 64-bit RISC-V 5-stage pipeline processor with the following stages:

- **Instruction Fetch (IF)**
- **Instruction Decode (ID)**
- **Execution (EX)**
- **Memory (MEM)**
- **Write-back (WB)**

It includes a basic forwarding unit and hazard detection logic.

A bubble sort program (in `sw/bubble_sort.c`) is provided and compiled using the RISC-V GCC toolchain. The resulting machine code (in Verilog hex format) can be loaded into memory for simulation.

