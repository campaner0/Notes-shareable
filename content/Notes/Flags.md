---
type: note
tags: [Embeded_Systems]
---
01/20/2023 14:45

  

For computer processors, status flags are used to indicate the status of results of operations. These flags are recored in the status register (see [[Computer Architecture]]). For the ARM Cortex-M, these are:
1. Negative (N) - set if result is negative
2. Zero (Z) - if result is 0
3. Overflow (V) 
4. Carry/Borrow (C)
5. Saturation (Q)


## Carry/Borrow Flags
If two unsigned integers are added and the result is too large for the register or less than zero, the flag is activated. If the operation crosses over to zero from the largest value possible for the register (addition), the carry flag is 1. If crosses from zero to the highest value (subtraction), it is set as 0. 

>[!info]
>If the carry bit is 1 after addition or 0 after subtraction, the result is wrong. If it is 0 after addition or 1 after subtraction, the answer is acceptable.

---

## Overflow
The overflow flag applies when working with signed integers. Overflow occurs when:
1. Two + integers added give a non-positive result
2. Two - added give non-negative 
3. Subtracting + from - gives + result
4. Subtracting - from + gives - result

>[!note]
>The [[CPU]] updates all flags whether or not the data is signed or unsigned. It only sees a binary number and it is up to the programer to decide if the data should be treated as signed or unsigned. 

---

## Updating Flags
Add the suffix 's' to the end of the mnemonic to update [[Flags]] at this operation. This is necessary when adding two numbers that are are larger than the register size or whose result will be larger. It can also used for comparison, to find out if a value is smaller or larger than another.

You can also use certain commands to execute an operation where only the flag matters, not the result. For example, to compare the values of two numbers. The operation will be executed and the flags updated, but the result is not stored. 

Instruction|Description|Flags
----|----|----
CMP|Compare|N, Z, C, V
CMN|Compare Negative|N, Z, C, V
TEQ|Test Equivalence|N, Z, C
TST|Test|N, Z, C
