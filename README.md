Bus-Based Architecture with RISC-V CPU in SystemVerilog
=======================================================

This project implements RISC-V microprocessor CPU based on the bus-based architecture. The processor is written Verilog HDL and includes a complete datapath, control flow simulation, and testbenches for each functional block. Simulation and verification were performed using **ModelSim**.



 ## Key Features
- Complete datapath with bus-based communication between units  
- Supports all major RISC-V instruction types (R, I, S, B, J)  
- Modular design including ALU, register file, memory, and control unit with mirco programming feature  
- Sign and zero extension units for immediate value handling  
- Control signals modeled as a 16-bit input to drive the datapath  
- Extensive testbenches for each module and the full datapath  



 ## Supported Instruction Types
- R-Type: Register-register arithmetic and logic operations  
- I-Type: Immediate arithmetic, logic, and load operations  
- S-Type: Store instructions for memory writes  
- B-Type: Conditional branches for control flow  
- J-Type: Unconditional jump instructions  



## Testbenches
- `ALU_test.v`  
- `TestMemory.v`  
- `RegisterTest.v`  
- `testSPR.v`  
- `TestSign.v`  
- `TestBench.v`  
- `ControlTest.v`  

---



## Results
- Successfully simulated all instruction types on the CPU  
- Verified correct datapath operation via modular testbenches  
- Achieved comprehensive coverage of control signals and data paths  

