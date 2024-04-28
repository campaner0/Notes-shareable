---
type: note
alias: GPIO
tags: [Embeded_Systems]
---
03/15/2023 14:45

  

For microcontrollers, GPIO is used to communicate with any peripheral such as LEDs, buttons, sensors, etc. Any communication with users or other devices happens through a GPIO port. This can happen with port-mapped or memory-mapped I/O, memory-mapped I/O is more commonly used because of its flexibility. Port-mapped I/O must use a special [[Assembly]] instruction.

Most [[CPU]]s do I/O using memory-mapped I/O. Each device register is given a memory address that is accessible by the CPU (in the memory space of the processor), so native load/store instructions can be used to communicate.


### Initialization



---
### PUPDR
The pull-up/pull-down register is used to read an input even through noise. If a switch to ground is connected to a GPIO pin, the processor will not be able to tell if it is open or closed due to noise. A pull up/down [[Resistance|Resistor]] (connected to high or ground respectivly) is used to clarify the signal. If a pull up resistor is used, when the switch shorts to ground, the input will be 0, but when it is open, the input will be pulled up by the [[Voltage]] source through the resistor.

Which one, if any, is used is decided by the value in the register:
1. 00 - Neither
2. 01 - Pull up
3. 10 - Pull down
4. 11 - Reserved

---

### Input Data Register (IDR)
