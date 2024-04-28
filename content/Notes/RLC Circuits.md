---
type: note
alias: RLC Circuit
---
04/11/2022 15:05

  #Circuit_Analysis, #Physics 

RLC circuits are circuits with resistors, capacitors, and inductors. They can be reduced to a single resistor, cap, and inductor. Its an LC circuit with a resistor ([[LC Circuits]]), which results in 
damping. 

### Damping
The Neper frequency, also called [[Attenuation]] or damping coeffiecient, it is how fast the transient response damps after the source is removed. It is denoted by $\alpha$. [[RLC Resonance|Resonant Frequency]] is denoted by $\omega_0$

when $\alpha>\omega_0$, the circuit is overdamped
when $\alpha=\omega_0$, the circuit is critically damped
when $\alpha<\omega_0$, the circuit is underdamped

---

### Parallel
For a parallel RLC circuit, the following differential equation results from using [[Kirchhoff's Current Law|KCL]] and simplifying:
$$
C\frac{d^2v}{dt^2}+\frac1R\frac{dv}{dt}+\frac vL=0
$$
where
- $C$ = [[Capacitance]]
- $R$ = [[Resistance]]
- $L$ = [[Inductance]]
- $v$ = [[Voltage]]
- $t$ = [[Time]]


##### Overdamped
For an overdamped circuit, the differential equation has this solution:
$$
v(t)=A_1e^{s_1t}+A_2e^{s_2t}
$$
where
$$\begin{matrix}
s_1=-\alpha+\sqrt{\alpha^2-\omega_0^2} \\
s_2=-\alpha-\sqrt{\alpha^2-\omega_0^2} \\
\end{matrix}$$

The circuit is overdamped when $\alpha>\omega_0$, therefore:
$$
R<\frac{1}{2C\omega_0}
$$
##### Critically Damped
For a critically damped circuit:
$$
v(t)=e^{-\alpha t}(A_1t+A_2)
$$

##### Underdamped
For an underdamped circuit, if $\alpha<\omega_0$, then:
$$v(t)=
\begin{cases}
e^{-\alpha t}(A_1e^{j\omega_dt}+A_2e^{-\omega_dt}) \\
e^{-\alpha t}(B_1\cos[\omega_dt]+B_2\sin[\omega_dt])
\end{cases}$$

where
$$\begin{matrix}
\omega_d=\sqrt{\omega_0^2-\alpha^2} \\
s_1=\alpha+\sqrt{\alpha^2-\omega_d^2}  \\
s_2=-\alpha+\sqrt{\alpha^2-\omega_d^2} \\
\end{matrix}$$

---

### Series
For a series RLC:
$$
L\frac{d^2i}{dt^2}+R\frac{di}{dt}+\frac 1Ci=0
$$
which is the dual of the equation for a parallel circuit. The solutions for each damping situation are the same, but for [[Current]] as a function of time instead of voltage.

---

### Settling Time
Settling time is how long it takes for a voltage peak to be $\le|0.01v_m|$, where $v_m$ is the first peak