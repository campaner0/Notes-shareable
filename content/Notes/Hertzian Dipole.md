---
type: note
---
02/05/2024 16:25

Tags: #Antennas #Electromagnetics 

The Hertzian dipole antenna is a type of omnidirectional antenna which consists of two linear conductors along the same axis, separated by a gap. Its length must be much less than the wavelength of its signal, and should not exceed $\lambda/50$.


## Far-Field Approximation
In the far-field, that is, when $R\gg\lambda$, the dipole's radiation is approximated by: 
$$\begin{align*}
\tilde{E}_{\theta} &= \frac{jI_{0}\ell k\eta_{0}}{4\pi}\left(\frac{e^{-jkR}}{R}\right)\sin\theta\\
\tilde{H}_{\phi} &= \frac{\tilde{E}_{\theta}}{\eta_{0}}
\end{align*}$$
where
- $\tilde{E}_{\theta}$ = time varying [[Electric Field]]
- $\tilde{H}_{\phi}$ = time varying [[Magnetic Field]]
- $I_0$ = [[Current]] amplitude
- $\ell$ = 
- $k$ = [[Wave Number]]
- $R$ = radial distance from origin
- $\theta$ = elevation angle (see [[Spherical Coordinates]])
- $\eta_0$ = [[Impedance]] of free space

### Power Density
the [[Poynting Vector|Power Density]] of a dipole is:
$$\begin{align*}
S(R,\theta)&= \frac{15\pi I_{0}^2}{R^2}\left(\frac{\ell}{\lambda}\right)^2\sin^2\theta\\[5pt]
&= S_0\sin^2\theta
\end{align*}$$
therefore the normalized radiation intensity $F(\theta)=\sin^2\theta$



