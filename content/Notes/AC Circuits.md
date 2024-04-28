---
type: note
tags: [Physics, Circuit_Analysis]
---
04/14/2022 12:39

 

AC circuits are circuits with [[Alternating Current]] sources

#### Power
see [[Electrical Power#AC|AC Power]]

#### Resistors
For a resistor circuit, the [[Voltage]] and [[Current]] are in phase. Current through the resistor is given by:
$$
i_R=\frac{V_{max}}{R}\sin\omega t=I_{max}\sin\omega t
$$
voltage follows [[Ohm's Law]] with the $\sin\omega t$ term

#### Inductors
In inductors, current and voltage are out of phase by -90$\degree$. This is the result of solving the differential equation that relates voltage and current for [[Inductance]]. Voltage is a sin wave, current is a cos wave. This can be written as:
$$
i_L=\frac{V_{max}}{\omega L}\sin\left(\omega{t}-\frac{\pi}2\right)
$$
where
- $\frac{\pi}2$ = [[Phase Angle]]

From this (in a circuit with only an inductor):
$$
I_{max}=\frac{V_{max}}{X_L}
$$
where
- $X_L=\omega L$ (Inductive [[Reactance]])

This formula also relates RMS voltage and current

#### Capacitors
Similarly to inductors, solving the differential equations in an AC context gives a phase shift of +90$\degree$.
$$
i_C=\omega CV_{max}\sin\left(\omega t+\frac{\pi}2\right)
$$
where
- $\frac{1}{\omega C}=X_C$ (Capacitive Reactance)