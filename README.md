Bus-Based Architecture with RISC-V CPU
======================================
This project implements a basic RISC-V microprocessor CPU based on the single-cycle architecture described in Chapter 4 of the Computer Organization and Design textbook. The processor is written in SystemVerilog and includes a complete datapath, control flow simulation, and testbenches for each functional block. Simulation and verification were performed using ModelSim.
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


Overview
The design includes the following core modules:

ALU: Handles arithmetic, logical, and shift operations.

Register File: Stores and retrieves data for general-purpose registers.

Memory: Word-addressable memory with instruction and data segmentation.

Special Purpose Registers: IR (Instruction Register), A, B, MA.

Sign/Zero Extension Unit: Extends immediate values based on opcode.

Datapath: Ties all components together under control signal sequences.
-----------------------------------------------------------------------

Supported Instruction Types
The CPU supports the following RISC-V instruction formats:

R-Type: Register-register arithmetic and logic operations

I-Type: Immediate arithmetic, logic operations, and loads

S-Type: Store instructions for memory write operations

B-Type: Conditional branch instructions for control flow

J-Type: Jump instructions for unconditional control flow
---------------------------------------------------------

Testbenches
All major modules have dedicated testbenches:

ALU_tb.sv

Memory_tb.sv

Register_file_tb.sv

Sign_extension_tb.sv

SP_Register_tb.sv

Datapath_tb.sv

control_test.sv

Testbenches cover standard and edge cases, and simulate multiple control signal combinations.
---------------------------------------------------------------------------------------------

Datapath Architecture
The datapath integrates:

Registers: A, B, IR, MA

Memory: Separated instruction/data space

Register File: Read/write capability with selector

ALU: Central computation unit

Control Signals: 16-bit input used to simulate instruction flow

Databus: A 32-bit shared bus to move values between units
---------------------------------------------------------------
