---
type: note
---
04/08/2022 14:29

Tags: #Circuit_Analysis, #Physics 

Impedance is the total opposition to current flow in a circuit. This includes resistance and the opposition due to (dis)charging capacitors and inductors. Though resistance is just one part of impedance, [[Ohm's Law]] still applies:
$$
\vec{Z}= \frac{\vec{V}}{\vec{I}}
$$
where
- $\vec Z$ = impedance
- $\vec V$ = [[Voltage]]
- $\vec I$ = [[Current]]

If the reactance of a circuit is known, the magnitude of the impedance can be found by:
$$
|\vec Z|=\sqrt{R^2+(X_L-X_C)^2}
$$
where
- $R$ = [[Resistance]]
- $X_L$ = inductive [[Reactance]]
- $X_C$ = capacitive reactance


This also works for [[Alternating Current#Root Mean Squared|RMS]] values

>[!note]
>When inductive and capacitive reactance are equal (e.g. zero, as in DC), impedance = resistance. In AC circuits, this only happens at a certain frequency (see [[RLC Resonance]])

---

## Impedance of Free Space

$$
Z_0=\sqrt{\frac{\mu_{0}}{\varepsilon_{0}}}
$$
