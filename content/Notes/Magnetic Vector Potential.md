---
type: note
tags: [Electromagnetics]
---
10/06/2022 17:33

  

The magnetic vector potential is the magnetic equivalent of [[Voltage]], or electric potential. However, it is a vector field, not a scalar field like electric potential. It is defined such that:
$$
\vec{B}=\nabla\times\vec{A}
$$
where
- $\vec{A}$ = magnetic vector potential
- $\vec{B}$ = [[Magnetic Field]]


A vector form of Poisson's equation exists, similar to the scalar equation for voltage:
$$
\nabla^2\vec{A}=-\mu\vec{J}
$$
where
- $\vec{J}$ = [[Current Density]]


It can also be found similarly to voltage due to a charge density:
$$
\vec{A}=\frac{\mu}{4\pi}\int_V\frac{\vec{J}}{R}dV
$$
where
- $\mu$ = [[Permeability]]
- $R$ = [[Distance]] between observation point (e.g. the origin) and measurement point
- $V$ = some [[Volume]]