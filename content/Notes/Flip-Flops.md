---
type: note
tags: [Digital_Logic]
---
10/17/2022 17:49

  

A flip-flop is the extension of latches to work with a clock pulse. They are constructed with a D Latch and an [[SR Latch]]:

![[Negative Edge Triggered D Flip-Flop.png]]
(Negative Edge Triggered Flip-Flop Pictured)

The clock functions to change the control input to only allow the memory to be changed either at the instant the clock goes high or low, depending on whether the flip-flop is negative-edge or positive-edge triggered. If, at the trigger, $D$ is the same value as the previous trigger, the output will not change.