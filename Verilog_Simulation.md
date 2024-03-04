# As per the Update given for the next task "Should Use the RISC-V Core Verilog netlist and testbench for functional Simulation.
# Veriog code is being executed and the waveforms are generated using the gtkwave

# Aim: To verify the Functional Simulation:-
# Table of contents
- [1.RISC-V RV32I](#1-RISC-V-RV32I)
 - [2.BLOCK DIAGRAM OF RISC-V RV32I](#2-BLOCK-DIAGRAM-OF-RISC-V-RV32I)
 - [3.INSTRUCTION SET OF RISC-V RV32I](#3-INSTRUCTION-SET-OF-RISC-V-RV32I)
 - [4.FUNCTIONAL SIMULATION](#4-FUNCTIONAL-SIMULATION)
    - [4.1 About iverilog and gtkwave](#41-About-iverilog-and-gtkwave)
    - [4.2 Installing iverilog and gtkwave](#42-Installing-iverilog-and-gtkwave)
    - [4.3 The output waveform](#43-The-output-waveform)
  
   ## 1. RISC-V RV32I

This project provides an insight into the working of a few important instructions of the instruction set of a Single cycle Reduced Instruction Set Computer - Five(RISC-V) Instruction Set Architecture suitable for use across wide-spectrum of Applications from low-power embedded devices to high-performance Cloud-based Server processors. The base RISC-V is a 32-bit processor with 31 general-purpose registers, so all the instructions are 32-bit long. Some Applications where the RISC-V processors have begun to make some significant threads are in Artificial intelligence and machine learning, Embedded systems, ultra-low power processing systems, etc.

## 2. BLOCK DIAGRAM OF R
![Screenshot 2024-03-04 213701](https://github.com/saad5738/Mohammed-Saad/assets/160725153/c98ed6d6-ca69-4479-848f-3342a10ab7e4)
ISC-V RV32I
3. INSTRUCTION SET OF RISC-V RV3
![Screenshot 2024-03-04 213730](https://github.com/saad5738/Mohammed-Saad/assets/160725153/b51e9eda-78b4-4f8f-8360-45db6d0cdca6)

![Screenshot 2024-03-04 213749](https://github.com/saad5738/Mohammed-Saad/assets/160725153/39914c4f-bbb4-4416-b660-d04905803619)
2I
## 4. FUNCTIONAL SIMULATION

### 4.1 About iverilog and gtkwave
- Icarus Verilog is an implementation of the Verilog hardware description language.
- GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.
  
### 4.2 Installing iverilog and gtkwave

- **For Ubuntu**

 Open your terminal and type the following to install iverilog and GTKWave
 ```
 $   sudo apt get update
 $   sudo apt get install iverilog gtkwave
 ```
![WhatsApp Image 2024-03-04 at 11 11 24_1c7b8e22](https://github.com/saad5738/Mohammed-Saad/assets/160725153/3129e3cd-8a48-4f3e-908b-233c7f76be3a)
- **To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.**

 ```
 $ git clone https://github.com/Saad5738/Mohammed-Saad
 $ cd Saad
```
![WhatsApp Image 2024-03-04 at 11 11 22_549aaf48](https://github.com/saad5738/Mohammed-Saad/assets/160725153/1a9e1c28-9659-4964-b866-ac1baec8b257)

- **To simulate and run the Verilog code, enter the following commands in your terminal.**

```
$ iverilog -o hello hello.v hello_tb.v
$ ./hello
```
![WhatsApp Image 2024-03-04 at 11 11 22_392733fa](https://github.com/saad5738/Mohammed-Saad/assets/160725153/50927bff-e179-441b-b674-79a75e69014b)
- **To see the output waveform in gtkwave, enter the following commands in your terminal.**

`$ gtkwave hello.vcd`
![WhatsApp Image 2024-03-04 at 11 11 24_a66e9560](https://github.com/saad5738/Mohammed-Saad/assets/160725153/c2308932-a1c1-4b2f-b930-852a3fcc6194)

### 4.3 The output waveform

 The output waveform showing the instructions performed in a 5-stage pipelined architecture.


 Instruction 1:add r6,r2,r1 
![Screenshot 2024-03-04 215758](https://github.com/saad5738/Mohammed-Saad/assets/160725153/8b45801f-296a-480b-8fc4-61db2436da02)

Instruction 2:sub r7,r1,r2
![Screenshot 2024-03-04 215817](https://github.com/saad5738/Mohammed-Saad/assets/160725153/8c52377b-5f1b-4fc9-b634-3a7e3b332d8a)

Instruction 3:and r8,r1,r3
![Screenshot 2024-03-04 215836](https://github.com/saad5738/Mohammed-Saad/assets/160725153/c9e11376-3c72-4d69-8b14-c2b0d7800d1e)

Instruction 4:or r9,r2,r5
![Screenshot 2024-03-04 215852](https://github.com/saad5738/Mohammed-Saad/assets/160725153/70cdeaac-3a85-48dc-bb98-426999704f1b)

Instruction 5:xor r10,r1,r4
![Screenshot 2024-03-04 220146](https://github.com/saad5738/Mohammed-Saad/assets/160725153/dbae01fd-ea6b-4ae4-9258-d3c54affb15d)

Instruction 6:slt r11,r2,r4
![Screenshot 2024-03-04 220203](https://github.com/saad5738/Mohammed-Saad/assets/160725153/c23d4f7e-18ab-4a13-a4d9-4cc6b90801e3)

Instruction 7:addi r12,r4,5
![Screenshot 2024-03-04 220218](https://github.com/saad5738/Mohammed-Saad/assets/160725153/e7bec2c1-aa63-4bc8-819f-042f3b1893ce)

Instruction 8:sw r3,r1,2
![Screenshot 2024-03-04 220236](https://github.com/saad5738/Mohammed-Saad/assets/160725153/70485c90-fcf1-4e40-b9b3-f20389a559e8)

Instruction 9:lw r13,r1,2
![Screenshot 2024-03-04 220249](https://github.com/saad5738/Mohammed-Saad/assets/160725153/bab1d4b2-e810-4759-a6a0-e42cd994a0df)

After branching, performing Instruction 11:add r14,r2,r2
![Screenshot 2024-03-04 220304](https://github.com/saad5738/Mohammed-Saad/assets/160725153/6200924c-afb1-410b-b95b-b3c724c5d57e)

![Screenshot 2024-03-04 220319](https://github.com/saad5738/Mohammed-Saad/assets/160725153/84100a05-422a-407e-8ba1-4f19be4b3b71)


Full 5-stage instruction pipeline and pc-increment description Waveform
![Screenshot 2024-03-04 220333](https://github.com/saad5738/Mohammed-Saad/assets/160725153/3b8402fa-7a31-44fa-9633-f4fedc0556e9)

![WhatsApp Image 2024-03-04 at 11 11 23_cf670c04](https://github.com/saad5738/Mohammed-Saad/assets/160725153/6056bdd0-b7be-4e11-af4f-8b077c7d66c8)

![WhatsApp Image 2024-03-04 at 22 15 54_ca4193ff](https://github.com/saad5738/Mohammed-Saad/assets/160725153/dbd9710c-f070-442e-9b33-c2d825ad2f3c)
