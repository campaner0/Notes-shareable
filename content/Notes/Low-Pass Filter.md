---
type: note
tags: [Comunication_Systems, Circuit_Analysis]
---
09/06/2023 14:47

  

A low-pass filter will [[Filters|Filter]] out frequencies above the corner [[Frequency]]. 

## First Order
A first order passive filter can be constructed with a resistor and cap in series, where the output is the voltage across the cap. 
![[Pasted image 20221116161451.png]]
The voltage across the cap will be the output, giving the [[Transfer Function]]:
$$\begin{align*}
H(s)&= \frac{\frac{1}{sC}}{\frac{1}{sC}+R}\\[5pt]
&= \frac{\frac{1}{CR}}{s+\frac{1}{CR}}
\end{align*}$$
with a corner frequency of 
$$
\omega= \frac{1}{RC}
$$

where
- $s$ = [[Complex Frequency]] where $\sigma=0$
- $C$ = [[Capacitance]]
- $R$ = [[Resistance]]
- $\omega$ = [[Angular Velocity|Angular Frequency]]

