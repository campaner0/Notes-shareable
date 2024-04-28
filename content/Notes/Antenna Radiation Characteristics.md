---
type: note
---
02/07/2024 15:50

  #Electromagnetics #Antennas 

An antenna's intensity of radiation in three dimensions is called its antenna pattern, and this directional pattern is described in terms of the normalized radiation intensity:
$$
F(\theta, \phi)=\frac{S(R,\theta,\phi)}{S_{max}}
$$
where
- $S$ = [[Poynting Vector|Power Density]] of antenna

>[!note]
>For highly directional antennas, $F$ may be plotted on a [[Decibels|Decibel]] scale


The pattern solid angle describes the width of the main lobe of the antenna pattern. 
$$
\Omega_{p} = \iint_{4\pi}F(\theta,\,\phi)\,d\Omega
$$
where
- $d\Omega=\sin\theta\,d\theta\,d\phi$ = [[Solid Angle]]

The wider the main lobe, the less directional the antenna pattern. This is measured by the directivity of the antenna pattern. It is the ratio of the maximum and average $F$ in all directions and is inversely proportional to $\Omega_p$: 
$$
\begin{align*}
D &= \frac{F_{max}}{F_{avg}}\\[5pt]
&= \frac{4\pi}{\Omega_{p}}
\end{align*}
$$

Another measure of the size of the main lobe is the half power (3dB) beamwidth, or the difference in angle between the two points where $F$ is half of its maximum:
$$
\beta=\theta_{2}-\theta_{1}
$$
where
- $\theta$ = half power angles, where $F(\theta,\,0)=0.5$ 

>[!note]
>For antennas with a single main lobe pointing in the $z$ direction, $\Omega_p$ is approximately the product of the half power beamwidths in the $xz$ and $yz$ planes:
>$$
>\Omega_{p}\approx\beta_{xz}\beta_{yz}
>$$

radiated power

$$
P_{rad}=R^{2}S_{max}\Omega_{P}
$$

radiation efficiency
$$
\xi={\frac{P_{\mathrm{rad}}}{P_{\mathrm{t}}}}
$$
where
- $P_t$ = transmitter/input power

Gain
$$
G=\xi D
$$

Antenna effective area

$$
\begin{align*}
A_{e} &= \frac{P_{int}}{S_{i}}\\[5pt]
&= \frac{\lambda^{2}D}{4\pi}
\end{align*}
$$
where
- $P_{int}$ = 
- $S_{i}$ = 
- $D$ = maximum linear dimension of antenna
- $\lambda$ = [[Wavelength]] 

Friis Transmission Formula
$$
\begin{align*}
\frac{P_{rec}}{P_{t}}&= \frac{\xi_{t}\xi_{r}A_{t}A_{r}}{\lambda^{2}R^{2}}\\
&= G_{t}G_{r}\left(\frac{\lambda}{4\pi R}\right)^2
\end{align*}
$$
where $P_{rec}$ = received power 