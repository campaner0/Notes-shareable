---
type: note
alias: AC
tags: [Circuit_Analysis]
---
03/28/2022 14:41

 

An oscillating [[Current]] source will produce a current that is described by a sinusoidal function:
$$
\Delta i=\Delta I_{max}\sin(\omega t+\phi)
$$
where
- $\omega$ = [[Angular Velocity|Angular Frequency]]
- $t$ = [[Time]]
- $\phi$ = [[Phase Angle]]

>[!note]
>The concept is the same for a voltage source, but the phase angle will be different between voltage and current for any circuit that is not purely reisistive

---

### AC Signal Properties
(see [[Waves]])
#### Phase
In an ac circuit, phase angle can be found by inverse tangent thanks to the frequency domain:
$$
\phi = \tan^{-1}\left(\frac{X_L-X_C}{R}\right)
$$
where
- $X_L$ = Inductive [[Reactance]]
- $X_C$ = Capacitive Reactance
- $R$ = [[Resistance]]

---

#### Root Mean Squared
"RMS" expresses AC [[Voltage]] or current in terms functionally equivalent to DC. A certain voltage RMS is the amount of AC voltage that would deliver the same power to a resistor as a DC source at that certain voltage. Also known as DC equivalent.
$$
V_{RMS}=\frac{|\vec{V}_p|}{\sqrt 2}
$$
where
- $V_p$ = peak voltage

---

#### Phasors
In frequency domain, current and voltage are [[Phasor|Phasors]] denoted by:
$$
\vec{I}=I_me^{j\phi}=I_m\angle\phi
$$
where
- $I_m$ = magnitude of current
- $\phi$ = phase angle

This is possible through [[Euler's Formula]], relating [[Sine|Sin]] and [[Cosine|Cos]] to a complex exponential.

Using this and the equation relating voltage and current in inductors and caps, the differential relationship becomes algebraic.

--  | Time Domain | Frequency Domain
-----------| ------------------|-------------
[[Resistance]] | $v=Ri$| $\vec{V}=R\vec{I}$
[[Inductance]] | $v_l=L\frac{di}{dt}$ | $\vec{V}=j\omega L\vec{I}$
[[Capacitance]] | $i_c=C\frac{dv}{dt}$ | $\vec{V}=\frac{1}{j\omega C}\vec{I}$

---

#### Impedance
[[Impedance]] is the AC equivalent of resistance. This is a complex value visible in the above table. The frequency domain equations are derived from [[Ohm's Law]]. Therefore the impedance for an inductor is $j\omega L$. 

