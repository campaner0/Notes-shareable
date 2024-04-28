---
type: note
tags: [Circuit_Analysis]
---
11/29/2022 12:12

  

Quality factor describes how underdamped an [[Waves|Oscillator]] or resonator is. In an [[RLC Circuits|RLC Circuit]], it is the ratio of [[Energy]] stored to energy lost. Circuits with a higher quality factor have a narrower [[Bandwidth]] and therefore greater frequency selectivity. The quality factor of a circuit operating at its resonant [[Frequency]] is given by:

#### Parallel
$$\begin{align*}
Q_{p}&=\omega_0RC=Q_{s}^{-1}\\[5pt]
&= R\sqrt{\frac{C}{L}}\\[5pt]
&= \frac{R}{|X_{C,0}|}=\frac{R}{|X_{L,0}|}
\end{align*}$$

#### Series
$$\begin{align*}
Q_s&=\omega_0\frac{L}{R}=Q_{p}^{-1}\\[5pt]
&= \frac{1}{R}\sqrt{\frac{L}{C}}\\[5pt]
\end{align*}$$

where
- $Q$ = quality factor at resonant frequency
- $\omega_0$ = [[RLC Resonance|Resonant Frequency]]
- $R$ = [[Resistance]]
- $C$ = [[Capacitance]]
- $X_{C,0}$ = capacitive [[Reactance]] at resonant frequency

