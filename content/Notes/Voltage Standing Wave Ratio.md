---
type: note
tags: [Electromagnetics, Antennas]
---
01/22/2024 17:10

  

The standing wave ratio for a certain [[Transmission Lines|Transmission Line]] voltage measures how well the load matches the line. It is the ratio of the maximum and minimum amplitudes of the voltage wave:
$$\begin{align*}
S&=\frac{|\widetilde{V}|_{max}}{|\widetilde{V}|_{min}}\\[5pt]
&= \frac{1+|\Gamma|}{1-|\Gamma|}
\end{align*}$$
where
- $\Gamma$ = [[Voltage Reflection Coefficient]]

The voltage maxima are found by evaluating $|\widetilde{V}(d_{max})|$ where $d_{max}$ is the distance from the load where the voltage is at a maximum. This distance is found by:
$$\begin{align*}
d_{max}&= \frac{\theta_r+2n\pi}{2\beta}\\[5pt]
&= \frac{\theta_r\lambda}{4\pi}+\frac{n\lambda}{2}
\end{align*}$$
where
- $\theta_r$ = [[Phase Angle]] of $\Gamma$ 
- $n\in\mathbb{N}\ge 1$ if $\theta_r<0$, otherwise $n\ge 0$ 
- $\beta$ = [[Wave Number]]
- $\lambda$ = [[Wavelength]]

The voltage minima occur at $d_{min}$, which can be found using $d_{max}$:
$$d_{min}=\begin{cases}
d_{max}+ \frac{\lambda}{4}\;\text{for}\;d_{max}\lt \frac{\lambda}{4}\\
d_{max}- \frac{\lambda}{4}\;\text{for}\;d_{max}\ge \frac{\lambda}{4}
\end{cases}$$
>[!note]
>Current minima occur at the same points as voltage maxima

