---
type: note
aliases:
  - Attenuation Coefficient
tags: [Circuit_Analysis]
---
11/29/2022 20:42

  

The [[Attenuation]] coefficient or "Neper Frequency," $\alpha$ (sometimes $\sigma$), describes how a signal is attenuated in a circuit. It has a unit of Nepers per second. A quantity $\alpha t$, where $t$ is time, is measured in Nepers, which are similar to [[Decibels]] in that it is a logarithmic scale: 
$$
L=\ln\left(\frac{x_1}{x_{2}}\right)
$$
where
- $L$ = attenuation in Nepers
- $x_1$ = measured signal
- $x_2$ = baseline

### Parallel RLC Circuit
The neper frequency for a parallel [[RLC Circuits|RLC Circuit]] is half of its bandwidth:
$$\begin{align*}
\alpha&=\frac{1}{2RC}\\[5pt]
&= \frac{1}{2}\mathcal{B}
\end{align*}$$
where
- $R$ = [[Resistance]]
- $C$ = [[Capacitance]]
- $\mathcal{B}$ = [[Bandwidth]]

---

### Series RLC Circuit
For a series circuit, the neper frequency is:
$$\begin{align*}
\alpha&=\frac{R}{2L}\\[5pt]
&= \frac{1}{2}\mathcal{B}
\end{align*}$$
where
- $L$ = [[Inductance]]

