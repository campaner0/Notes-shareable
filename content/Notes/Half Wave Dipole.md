---
type: note
---
02/19/2024 16:44

Tags: #Antennas #Electromagnetics 

A half wave dipole is a dipole antenna where the length of the antenna is half the wavelength of its signal.

## Far-Field Approximation
$$\begin{align*}
\tilde{E}_{\theta}&= j60I_{0}\left[\frac{\cos(\pi/2\cos\theta)}{\sin\theta}\right]\left(\frac{e^{-jkR}}{R}\right)\\
\tilde{H}_{\phi}&= \frac{\tilde{E}_{\theta}}{\eta_{0}}
\end{align*}$$
where
- $\tilde{E}_{\theta}$ = time varying [[Electric Field]]
- $\tilde{H}_{\phi}$ = time varying [[Magnetic Field]]
- $I_0$ = [[Current]] amplitude
- $\theta$ = elevation angle (see [[Spherical Coordinates]])
- $k$ = [[Wave Number]]
- $R$ = radial distance from origin
- $\eta_0$ = [[Impedance]] of free space

### Power Density
The [[Poynting Vector|Power Density]] is given by:
$$\begin{align*}
S(R,\theta)&= \frac{15I_{0}^{2}}{\pi R^{2}}\left[\frac{\cos(\pi/2\cos\theta)}{\sin\theta}\right]^{2}\\[5pt]
&= S_{0}\left[\frac{\cos(\pi/2\cos\theta)}{\sin\theta}\right]^{2}
\end{align*}$$

It follows that the normalized radiation intensity is:
$$
F(\theta)=\left[{\frac{\cos(\pi/2\cos\theta)}{\sin\theta}}\right]^{2}
$$