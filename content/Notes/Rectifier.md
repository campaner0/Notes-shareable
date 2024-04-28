---
type: note
alias: Rectifiers
tags: [Circuit_Analysis]
---
02/14/2023 10:14

  

Rectifiers are circuits that "rectify" an [[Alternating Current|AC]] input to an approximate DC output. 


## Half-Wave Recitfier
50% power loss


---

## Full-Wave Rectifier

$$
V_{ripple}= \frac{V_{m}}{f_{out}R_{load}C_{}}
$$
where
- $V_m$ = peak output [[Voltage]]
- $f$ = [[Frequency]]
- $R$ = [[Resistance]] 
- $C$ = [[Capacitance]] of smoothing cap

>[!note]
>Since the trough of the input signal is rectified to a peak, the frequency of the output of a full wave rectifier is double the input


### Full-Wave Bridge Rectifier
A full-wave bridge rectifier uses four diodes in a bridge configuration to reduce the peak inverse voltage the diodes experience by about half compared to a center tapped design, with ideal diodes. This greatly increases diode stability and saftey with diodes that have a lower PIV tolerance. 