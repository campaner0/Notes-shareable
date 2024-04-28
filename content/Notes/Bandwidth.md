---
type: note
---
11/29/2022 12:12

Tags: #Circuit_Analysis 

The bandwidth of a [[RLC Resonance|Resonant RLC Circuit]] is the width of the portion of the [[Response Curve]] of the circuit that is $\ge$ the maximum, or the difference of the half-power frequencies:
$$\begin{align*}
\mathcal{B}&=\omega_2-\omega_1\\[5pt]
&= \frac{\omega_0}{Q_0}
\end{align*}$$
where
- $\omega_1$ = lower half power frequency
- $\omega_2$ = upper half power frequency
- $\omega_0$ = resonant frequency
- $Q_0$ = [[Quality Factor]]


### Half Power Frequencies
The half power frequencies are the frequencies where the input [[Conductance|Admittance]] magnitude > admittance at the resonant frequency by a factor of $\sqrt 2$. They can be calculated by:
$$
\omega_{1,2}=\omega_0\left[\sqrt{1+\left(\frac{1}{2Q_0}\right)^2}\mp \frac{1}{2Q_0}\right]
$$

>[!info]
>The resonant frequency can also be calculated from the half power frequencies if the quality factor is known:
>$$
\omega_0=\sqrt{\omega_1\omega_2}
$$

---

### High-Q Circuits
For circuits with a quality factor $Q_0\ge5$, several approximations can be made for finding the resonant and half power frequencies:
$$\begin{align*}
\omega_{1,2}&\approx\omega_0\mp \frac{1}{2}\mathcal{B}\\
\omega_0&\approx\frac{1}{2}(\omega_1+\omega_2)
\end{align*}$$