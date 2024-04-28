---
type: note
---
01/11/2023 14:53

Tags:  #Embeded_Systems 

Computer architecture refers to how data is stored in [[Memory]] (such as [[RAM]]) and how the data is moved around and processed within the computer. 

## Memory
There are two main memory architectures used:

### Von Neumann
In the Von Neumann architecture, instruction/address and data are stored in the same memory device. Therefore there is one data/address bus 

### Harvard
The Harvard architecture uses a different memory device for instructions and data and distinct data and address busses.

---

## Bus



---

## Registers
Registers are a type of memory that is built into the microprocesser itself. These are the fastest way to read/write, and are used because the cpu cannot access the memory directly. For example, the ARM Cortex-M has 13 general purpose registers (R0-R12), 3 special registers (R13-R15), and some others:

- Stack Pointer (R13) -
- Link Register (R14) - holds address to return to after running subroutine. LSb is always 1 for ARM Cortex-M to indicate Thumb processor mode 
- PC register (R15) - holds the location for the next instruction to fetch from memory. This is always incremented by 4

The registers function with the [[CPU]] to execute the cycle below:

![[Pasted image 20230113145544.png]]

This cycle can happen simultaneously in different registers. For example, one fetches the next instruction while another register decodes the current one, and so on for each register every clock cycle. This is called the Three-State Pipeline

### Processor Registers



---

### Peripheral Registers



---

### Load-Modify-Store
The process of loading data into the register from memory, modifying, and storing the data is described below.

The process for adding 1 to a variable:
1. Register R0 holds memory address of variable
2. Variable data is loaded from memory into R1.
3. Computation takes place, stored in R1
4. The result is saved to memory from R1