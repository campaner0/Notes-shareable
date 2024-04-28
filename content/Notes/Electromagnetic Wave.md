---
type: note
---
04/19/2022 13:36

  #Physics 

Also known as light, electromagnetic waves consist of a traveling [[Electric Field|Electric]] and [[Magnetic Field]]. The properties of the wave depend on the permittivity, permiability, and [[Conductivity]] of the medium it is traveling through. If the medium does not conduct, it is said to be lossless as it does not [[Attenuation|Attenuate]] the wave.

### Homogenous Wave Equations
By taking the [[Curl]] of both sides of Faraday's Law for time-varying waves and rewritting using an identity, an equation for the [[Electric Field|Electric]] and [[Magnetic Field]] can be found:
$$\begin{align*}
\nabla^2\widetilde{E}-\gamma^2\widetilde{E}&=0\\
\nabla^2\widetilde{H}-\gamma^2\widetilde{H}&=0
\end{align*}$$
where
- $\gamma=-\omega^2\mu\varepsilon_c$ 
	- $\omega$ = [[Angular Velocity|Angular Frequency]]
	- $\mu$ = [[Permeability]]
	- $\varepsilon_c$ = [[Permittivity|Complex Permittivity]]


---

### Phase Velocity
An electromagnetic wave's phase velocity in a vacuum is equal to [[Speed of Light]]:
$$
u_p=c= \frac{1}{\sqrt{\mu_0\varepsilon_0}}
$$
where
- $\varepsilon_0$ = vacuum [[Permittivity]]
- $\mu_0$ = vacuum [[Permeability]]

In another medium, the phase velocity would be dependent on the relative permittivity and permeability of the medium:
$$
u_p= \frac{c}{\sqrt{\mu_r\varepsilon_r}}=\frac{1}{\sqrt{\mu_r\mu_0\varepsilon_r\varepsilon_0}}
$$

---

### Momentum of Light
Any particle with no mass travels at the speed of light. This is derived from [[Special Relativity|Einstein's Equation]], which gives:
$$
p=\frac {T_{ER}}c
$$
where
- $p$ = [[Momentum]]
- $T_{ER}$ = [[Energy]]

Therefore if a surface absorbs a photon, it aquires its momentum, but if it reflects a photon, it aquires twice the momentum.

For complete absorption:
$$
P=\frac Sc
$$
For complete reflection:
$$
P=\frac{2S}c
$$
where $P$ is the power delivered to the object. 

In general:
$$
P=(1+f)\frac Sc
$$
where
- $f$ = reflection constant of material (1 being perfect reflection, 0 perfect absorption)