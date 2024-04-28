---
type: note
tags: [Digital_Logic]
---
10/24/2022 17:42

  

A sequential circuit is a circuit in which both the outputs and next state of the circuit depend on the inputs and present state of the circuit. That is, the outputs influence the the state of the circuit, along with inputs. 

>[!example]
>![[Pasted image 20221024174612.png]]
>
>where:
>$$\begin{align*}D_A&=AX+BX\\
>D_B&=\bar{A}X\\
>Y&=(A+B)\bar{X}\end{align*}$$
>This example utilizes D [[Flip-Flops]] and a clock, meaning it updates each clock cycle.

### State Tables
Each sequential circuit has a corresponding state table that describes the current and next state of the circuit according to the inputs and outputs. It is formatted like a truth table. The state table for the above example is:

![[Pasted image 20221024175500.png]]

---

### State Diagrams
