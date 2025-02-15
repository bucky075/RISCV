# 64-bit RISC-V 5-stage Pipeline

This project implements a simplified 64-bit RISC-V 5-stage pipeline processor with the following stages:

- **Instruction Fetch (IF)**
- **Instruction Decode (ID)**
- **Execution (EX)**
- **Memory (MEM)**
- **Write-back (WB)**

It includes a basic forwarding unit and hazard detection logic.

A bubble sort program (in `sw/bubble_sort.c`) is provided and compiled using the RISC-V GCC toolchain. The resulting machine code (in Verilog hex format) can be loaded into memory for simulation.

## Directory Structure

my-riscv-pipeline/ ├── .devcontainer │ ├── devcontainer.json │ └── Dockerfile ├── rtl │ ├── top.v │ ├── if_stage.v │ ├── id_stage.v │ ├── ex_stage.v │ ├── mem_stage.v │ ├── wb_stage.v │ ├── forwarding_unit.v │ └── hazard_detection_unit.v ├── testbench │ └── cpu_tb.v ├── sw │ ├── bubble_sort.c │ └── Makefile ├── scripts │ └── run_sim.sh └── README.md
