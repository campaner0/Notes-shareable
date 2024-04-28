---
type: note
---
04/05/2023 14:49

Tags: #Embeded_Systems 

The system timer (SysTick) keeps track of time in a [[CPU]]. At every tick, an [[Interrupts|Interrupt]] is generated that runs SysTick_Handler. These ticks are defined as an arbitrary amount of clock cycles. The time between ticks can be modified by slowing the clock or changing the value in the reload value register.

## Registers

1. Control/Status - SysTick_CTRL
2. Reload - SysTick_LOAD
3. Current value - SysTick_VAL
4. Calibration - SysTick_CALIB