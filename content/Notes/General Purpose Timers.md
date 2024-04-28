---
type: note
alias: General Purpose Timer
---
04/10/2023 15:18

  #Embeded_Systems 

The general purpose timers on a microcontroller are designed by the chip's designer and may vary from chip to chip. This is as opposed to the [[System Timer]], which is a standard peripheral designed by ARM. Whereas the system timer is specialized in nature, general purpose timers are can be used for a variety of applications.



### Input Capture
For a digital input, the harware edge detector can trigger an [[Interrupts|Interrupt]], but it can also trigger the timer value to be recorded in the CCR. This can be used to find the period of a digital signal.

#### DIER
Timer DMA Interrupt Enable Register is used to enable interrupts that can be triggered by the timer. 