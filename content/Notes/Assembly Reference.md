---
type: note
---
02/15/2023 15:10

Tags: #Embeded_Systems 


## Example Program
```Assembly
		AREA example_code, CODE, READONLY ;code header, required
		EXPORT _main
		ALIGN
		ENTRY
_main   PROC
		...
		...
		ENDP

		AREA example_data, DATA, READWRITE ;data header, required if program creates
		ALIGN                              ; data
		...
		...

		END
```

## Common Instructions

### Arithmetic

![[Pasted image 20230201145144.png]]

>[!note]
>If the destination register is the same as the first value in the operation, it may only be written once. For example:
>`ADD r1, r3` and `ADD r1, r1, r3` are both `r1 = r1 + r3`

>[!example]
>```start
>; Two 64 bit integers A (r1, r0) and B (r2, r3) with 32 bit register 
>; result C (r4, r5)
>; A = 00000002FFFFFFFF
>; B = 0000000400000001
>	LDR r0, =0xFFFFFFFF
>	LDR r1, =0x00000002
>	LDR r2, =0x00000001
>	LDR r3, =0x00000004
>; Add A to B
>	ADDS r4, r2, r0 ; update carry
>	ADC r5, r3, r1 ; add with carry
>	
>stop B stop
>```

---

### Bitwise Logic

![[Pasted image 20230203143724.png]]

>[!warning]
>Bitwise logic is not the same as Boolean logic. Boolean opeates on entire words while bitwise operates on individual bits. 

---

### Branch Instructions

![[Pasted image 20230222144508.png]]

---
## Suffixes

### Condition Codes
Condition codes modify an instruction so that it only executes if the applicable [[Flags]] are in the right state. 

![[Pasted image 20230217144756.png]]

