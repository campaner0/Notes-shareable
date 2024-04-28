---
type: note
alias: Interrupt
tags: [Embeded_Systems]
---
03/24/2023 15:09

  

Interrupts generate a request to the [[CPU]] to change the task the CPU is running. This opposed to polling, where the CPU is contantly reading the IDR (see [[General Purpose Input Output|GPIO]]) to see if a certain bit is set. For interrupts, the harware generates a service request when necessary so that the CPU can work on other tasks. When the CPU recieves a request, it stops the current code and runs an Interrupt service routine (ISR).


### NVIC
The Nested Vectored Interrupt Controller manages all interrupt requests that come in from software or hardware. It handles:
- whether to enable/disable interrupts
- interrupt priority
- locating interrupt's corresponding ISR
- resuming suspended code

When an interrupt occurs, registers r0 - r3 and r12 - r15 plus the xPSP register are automatically pushed to the currently selected [[Stack]], then the interrupt handler takes over. When it is done, it automatically unstacks. Other registers must be stacked/unstacked manually if they need to be preserved. The [[Computer Architecture#Registers|Link Register]] indicates is MSP or PSP is used:

![[Pasted image 20230329151316.png]]


The controller manages interrupts with their control bits which are stored in six registers:

![[Pasted image 20230331144722.png]]

>[!note]
>To disable an interrupt, the disable bit must be set to 0. Changing the enable bit will not disable it. Same for pending/unpending


#### Priority
Interrupt priority is adjusted by interrupt priority register: IP.

#### External Interrupts
These are triggered by external input (buttons, sensors). Each controller supports 16 external interrupt inputs, each one on a specific pin. Each interrupt can be assigned a pin, which is done on the chip using a [[(De)multiplexer|Multiplexer]]. 