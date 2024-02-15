# CS61CPU - A 32-bit RISC-V CPU

This repository contains my work for the CS61C Fall 2022 Project 3, where I designed and implemented a 32-bit CPU based on the RISC-V instruction set architecture. This project was a hands-on opportunity to apply the concepts learned in CS61C, including computer architecture, digital logic design, and RISC-V assembly programming.

## Project Overview

The CS61CPU is a single-cycle processor capable of executing a subset of the RISC-V instruction set. The design was implemented using Logisim, a graphical tool for designing and simulating digital logic circuits. This project was completed as part of the CS 61C course at the University of California, Berkeley.

For detailed project specifications and guidelines, visit the [official project website](https://inst.eecs.berkeley.edu/~cs61c/fa22/projects/proj3/).

## Features

- **Arithmetic Logic Unit (ALU):** Supports basic arithmetic and logical operations such as addition, subtraction, AND, OR, XOR, and shifts.
- **Register File:** A set of 32 registers for storing intermediate computation results.
- **Immediate Generator:** Generates immediate values from instructions for operations like `addi`.
- **Control Logic:** Determines the operation of the ALU, the data flow, and the write-enable signals based on the current instruction.
- **Datapath:** Integrates all components (ALU, Register File, Immediate Generator, Control Logic) to execute instructions.

## Implementation Details

- **Part A: Basic CPU Design**
  - Implemented ALU operations including `add`, `sub`, `and`, `or`, `xor`, `sll`, `srl`, and `sra`.
  - Designed a register file with read and write capabilities.
  - Created an immediate generator for `addi` instructions.
  - Assembled the datapath to execute the `addi` instruction.

- **Part B: Extended CPU Design**
  - Extended the ALU and control logic to support additional RISC-V instructions such as load, store, branch, and jump instructions.
  - Implemented pipelining to improve instruction throughput.
  - Added support for handling hazards and implemented control logic for branch prediction.

## Challenges and Learning Outcomes

- **Digital Logic Design:** Gained hands-on experience with designing complex digital circuits.
- **RISC-V ISA:** Deepened understanding of the RISC-V instruction set and its execution on hardware.
- **Computer Architecture Concepts:** Applied concepts such as pipelining, hazard detection, and control logic in a practical project.
