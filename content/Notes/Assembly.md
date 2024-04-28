---
type: note
---
01/27/2023 14:44

  #Embeded_Systems 

Assembly, the assembly language, machine language or machine code, is the lowest level human-readable programming language. It describes the basic processes of the [[CPU]]: moving data and operating on it, arithmetic, comparison, interrupts, etc. 

## Instruction Formats
Different assemblers may format instructions differently. The general format is:

`Label mnemonic operand1 operand2 operand3 ; comments`

Other formats may separate the end of the line and comments with `@`, `\\`, or `/* */`

- Labels are optional, but are used to implement [[If-Then Statements]] and [[Loops]]. They mark the [[Memory]] address of the current instruction and must be unique within the file.
- The mnemonic is the name of the instruction.
- Operands may be the name of a register or an immediate value ([[Constant]]). There may be no operands or many, but the first is usually the destination register, the second and third being source registers, immediate values, registers shifted by x bits, or a register plus an offset. 
- Comments appear after the machine code, separated by a symbol that ends the line. These are used to explain the programmer's intentions/assumptions.

---

## Loading, Storing Data
When working with data longer that 1 byte, the load and store instructions may be fed an offset to reference the data in a halfword, word, etc that is not stored at the word's address. The offset may be an immediate value or data stored in a register. This can be done in multiple ways:

### Pre-Index
`LDR r1, [r0, #4]`

Pre-index syntax causes the data in r1 to be loaded from/stored at the address in r0 + 4. If r0 was 0x2000800, then the data would be stored at 0x2000804. The address stored in r0 is not changed.


### Post-Index
`LDR r1, [r0], #4`

Post-index causes the data in r1 to be stored at the address in r0, then the address in r0 is updated to r0 + 4.


### Pre-Index with update
`LDR r1, [r0, #4]!`

Pre-index with update is a combination of the previous two. The data in r1 is stored at r0 + 4 and r0 is updated to r0 + 4.

---

## Control Structures

- Sequence Structure: The computer executes sequential instructions, one after another.
- Selection Structure: Two or more instruction paths are available based on a condition.
- Loop Structure: Repeat the same action over and over while a condition is true, checking after each loop.


---

## Branching
Branching in assembly is how if/then, cases and loops are implemented. There are two types of branch instructions: unconditional and conditional.

### Unconditional
Unconditional branch instructions will jump to the stated label when the program reaches that instruction no matter what.
- `B`  
- `BL` - used to jump to a subroutine/function
- `BLX` - 
- `BX` - used to return from function to main process using address in link register
	- any values passed back will first be written to r0, then others

---

### Conditional 
Conditional branching uses [[Assembly Reference#Condition Codes|Condition Codes]] along with the compare instructions to decide whether to jump or not. 

>[!example]
>

---
## Miscellaneous Syntax

```
r1 ; refers to data in register 1
[r1] ; refers to address of r1
#3 ; immediate value 3
ADDS ; same as ADD, but S updates flags
```




