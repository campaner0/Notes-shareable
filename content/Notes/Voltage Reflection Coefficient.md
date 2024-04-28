---
type: note
---
11/10/2022 17:25

  #Electromagnetics 

The voltage reflection coefficient is the ratio of the amplitudes of the reflected and incident voltage waves at the load of a [[Transmission Lines|Transmission Line]] circuit:
$$\begin{align*}
\Gamma=\frac{V_0^-}{V_0^+}&= \frac{Z_L-Z_0}{Z_L+Z_0}\\
&= \frac{z_L-1}{z_L+1}
\end{align*}$$

where
- $\Gamma$ = [[Voltage]] reflection coefficient
- $V_0^+$ = incident wave amplitude
- $V_0^-$ = reflected wave amplitude
- $Z_L$ = load [[Impedance]]
- $z_L={Z_L}/{Z_0}$ = normalized load impedance


The load impedance of a transmission line is the ratio of voltage and current at that point ($z=0$). Using the solutions to the wave equations above and manipulating will result in the ratio of the amplitudes of the incident and reflected voltages, or the voltage reflection coefficient. It is a measure of how much of the incident wave is reflected by the load.

>[!info]
>$\Gamma=0$ when a load is matched to a transmission line, that is, when $Z_L=Z_0$. This is because there are no travelling waves 
>
>$\Gamma=1$ when $Z_L=\infty$, that is, with an open circuit load
>
>$\Gamma=-1$ when $Z_L=0$, that is, with a short circuit load

