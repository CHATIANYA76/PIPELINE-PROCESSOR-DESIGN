# PIPELINE-PROCESSOR-DESIGN

COMPANY : CODTECH IT SOLUTIONS

NAME : KULLAPPA CHAITANYA

INTERN ID : CT04DM114

DOMAIN : VLSI

MENTOR : NEELA SANTOSH

*DESCRIPTION OF THE TASK :

The provided VHDL code implements a simplified model of a pipelined processor architecture using a behavioral approach. This design simulates a basic instruction pipeline with four main stages: Instruction Fetch (IF), Instruction Decode (ID), Execute (EX), and Write Back (WB). The processor is triggered by the rising edge of a clock signal and operates sequentially through these stages, allowing instructions to be executed in a step-by-step fashion. The code is designed for educational and illustrative purposes and models the functioning of a basic processor that handles a small instruction set, including operations such as ADD, SUB, and LOAD.

The processor uses a small set of general-purpose registers and a limited memory block. The register file consists of four 8-bit registers declared as an array of standard logic vectors. Similarly, a memory array of sixteen 8-bit locations stores the instructions and data. Instructions are 8 bits wide, and the encoding scheme uses the upper two bits for the opcode and the remaining bits to denote source and destination registers. The instruction format divides the 8-bit instruction into four 2-bit fields: opcode (bits 7-6), destination register (bits 5-4), source register 1 (bits 3-2), and source register 2 or address (bits 1-0).

The Instruction Fetch (IF) stage retrieves the instruction from memory based on the current value of the Program Counter (PC) and updates the PC for the next instruction. In the Instruction Decode (ID) stage, the instruction fetched in the previous cycle is decoded into its constituent fields: opcode, destination, and source registers. These decoded values are then used in the Execute (EX) stage to perform the actual operation. The source registers are read from the register file and depending on the opcode, an arithmetic or memory load operation is performed. For ADD and SUB instructions, the values from the two source registers are added or subtracted using unsigned arithmetic. For LOAD instructions, data is loaded directly from the memory using one of the source fields as the address.

OUTPUT:

<img width="786" alt="Image" src="https://github.com/user-attachments/assets/12eabff8-afe6-471b-8f3d-f9f23cae9636" />
