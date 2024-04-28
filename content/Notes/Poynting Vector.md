---
type: note
aliases:
  - Power Density
---
10/27/2022 17:37

  #Physics #Electromagnetics 

The Poynting [[Vector]] denotes the direction and intensity (or power flow) of an [[Electromagnetic Wave]]. It has units of $\text{W/m}^2$, therefore it represents the power density of the wave. 
$$
\vec{S}\equiv\frac 1{\mu_0}\vec{E}\times\vec{B}
$$
where
- $\vec{S}$ = Poynting Vector
- $\vec{E}$ = [[Electric Field]]
- $\vec{B}$ = [[Magnetic Field]]
- $\mu_0$ = vacuum [[Permeability]]

The intensity $I$ is the time average of the Poynting vector:
$$\begin{align*}
\vec{I}=\vec{S}_{avg}&= \frac{1}{2}\mathfrak{Re}(\tilde{E}\times\tilde{H}^*)\\[5pt]

\end{align*}$$
Its magnitude is calculated using rms or maximums and can be written in terms of one field using their relation to the speed of light ([[Maxwell's Equations#The Wave Equation|The Wave Equation]]):
$$\begin{align*}
|\vec{I}|&= \frac{E_mB_m}{2\mu_0}\\[5pt]
&= \frac{E_m^2}{2\mu_0c}=\frac{cB_m^2}{2\mu_0}
\end{align*}$$

The magnitude of the Poynting vector multiplied by an area gives the [[Electrical Power]] delivered by the light in that area. Multiply again by [[Time]] to get [[Energy]]
