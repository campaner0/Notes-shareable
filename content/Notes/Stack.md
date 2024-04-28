---
type: note
---
02/24/2023 14:34

  #Embeded_Systems 

The stack is used to save the contents of the registers at the start of a [[Function|Subroutine]] so that the registers may be used by the function. The contents are restored after. It may also be used to pass more arguments than r0-r4 can hold or to save the contents of the registers in the event of an interrupt. The stack operates in a last-in-first-out model. Only the item most recently added may be accessed. 

In memory, the stack may grow from top to bottom or bottom to top. These are the descending and ascending growth conventions. 

>[!note]
>The ARM Cortex-M uses full descending stack


## Push and Pop
"Pushing" data means to add it to the stack and "pop" means to remove data from the stack back into registers. Registers r0 - r12 and the link register can be pushed or popped, but PC register can only be popped to, not pushed. The registers will be pushed or popped in ascending order (r0 to r15).

Syntax:
```
PUSH {register list}
POP {register list}
```



>[!note]
> The list of registers may be in any order, but the lowest number register is stored/retrieved to/from the lowest memory address. This means the lowest register is stored last and loaded first

---
## Stack Pointer
The stack pointer keeps track of how "high" the stack is and may point to the last item or the memory address after the last item. 

The register SPSEL can select between the Main Stack Pointer and Process Stack Pointer depending on if the processer is in thread or handler mode. 