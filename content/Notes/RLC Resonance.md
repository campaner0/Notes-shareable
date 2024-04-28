---
type: note
tags: [Circuit_Analysis]
---
11/14/2022 15:56

  

At certain frequencies the [[Impedance]] phasors of the cap and inductor in an RLC circuit are 180$^\circ$ apart, so they cancel each other out which results in a purely real impedance, the equivalent [[Resistance]] of the circuit. This occurs when the [[Voltage]] and [[Current]] inputs are in phase, which is at resonant frequencies:
$$\begin{align*}
\omega_0&=\frac{1}{\sqrt{LC}}\\[5pt]
&= \sqrt{\omega_1\omega_2}
\end{align*}$$
where
- $\omega_0$ = resonant [[Frequency]]
- $\omega_{1,2}$  = [[Bandwidth|Half Power Frequencies]]
- $L$ = [[Inductance]]
- $C$ = [[Capacitance]]

>[!note]
>The resonant frequency is used, along with the [[Neper Frequency|Attenuation Coefficient]], in [[RLC Circuits]] to determine if the circuit is under/over/critically damped

### Parallel Resonance
For a parallel [[RLC Circuits|RLC Circuit]], the following equations are true:
$$\begin{align*}
|\vec{I}_L(j\omega_0)|=|\vec{I}_C(j\omega_0)|=Q_0|\vec{I}(j\omega_0)|\\[5pt]
\vec{Y}=\frac{1}{R}\left[1+jQ_0\left(\frac{\omega}{\omega_0}-\frac{\omega_0}{\omega}\right)\right]
\end{align*}$$

---

### Series Resonance
The equivalents for a series circuit:
$$\begin{align*}
|\vec{V}_L(j\omega_0)|=|\vec{V}_C(j\omega_0)|=Q_0|\vec{V}(j\omega_0)|\\[5pt]
\vec{Z}=R\left[1+jQ_0\left(\frac{\omega}{\omega_0}-\frac{\omega_0}{\omega}\right)\right]
\end{align*}$$
where
- $\vec{I}$ = [[Current]]
- $\vec{V}$ = [[Voltage]]
- $\vec{Y}$ = input [[Conductance|Admittance]]
- $\vec{Z}$ = input [[Impedance]]
- $R$ = [[Resistance]]
- $Q_0$ = [[Quality Factor]]
- $\omega$ = [[Angular Velocity|Angular Frequency]]

---

### Aproximations
For circuits with a high quality factor ($5$ or above), the following approximations can be made:
$$\begin{array}{c|c}
\text{Parallel}&\text{Series}\\
\hline
\vec{Y}\approx \frac{1}{R}\sqrt{1+N^2}\angle\tan^{-1}N&\vec{Z}\approx R\sqrt{1+N^2}\angle\tan^{-1}N
\end{array}$$
where
- $N= \large\frac{\omega-\omega_0}{\frac 12\mathcal{B}}$ = number of half [[Bandwidth|Bandwidths]] from resonance

---

### Other Forms
