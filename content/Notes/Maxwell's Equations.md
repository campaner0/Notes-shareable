---
type: note
---
04/19/2022 13:13

Tags: #Physics 

Maxwell's equations are these four relating to electromagnetism:

[[Gauss's Law]]

[[Faraday's Law of Induction]]

[[Magnetic Flux#Gauss's Law in Magnetism|Gauss's Law in Magnetism]]

[[Ampere's Law]]


### Electro/Magnetostatics
When [[Charge]] (and therefore [[Current]]) is zero, the equations become:
$$
\oint\vec{E}\cdot d\vec{l}=0
$$
$$
\int\vec{B}\cdot d\vec{A}=0
$$
$$
\int\vec{E}\cdot d\vec{s}=-\frac{d\Phi_B}{dt}
$$
$$
\int\vec{B}\cdot d\vec{s}=\varepsilon_0\mu_0\frac{d\Phi_E}{dt}
$$
Differential forms:
$$
\nabla\cdot\vec{D}=\rho_v
$$
$$
\nabla\cdot\vec{B}=0
$$
$$
\nabla\times\vec{E}=-\frac{\partial\vec{B}}{\partial t}
$$
$$
\nabla\times\vec{H}=\vec{J}+\frac{\partial\vec{D}}{\partial t}
$$
where
- $\vec{E}$ = [[Electric Field]]
- $\vec{B}$ = [[Magnetic Field]]
- $\vec{D}$ = [[Electric Displacement Field]]
- $\vec{H}$ = [[Magnetic Field Strength]]
- $\vec{J}$ = [[Current Density]]
- $\Phi$ = [[Electric Flux]] or [[Magnetic Flux]]
- $\varepsilon$ = [[Permittivity#Vacuum Permittivity|Vacuum Permittivity]]
- $\mu$ = [[Permeability]]
- $\nabla$ = [[Gradient]] operator
- $\rho_v$ = [[Charge Distribution]] (volume)

---

### Electro/Magnetodynamics
For sinusoidal time variation:
$$\begin{align*}
\nabla\cdot\widetilde{E}&=\frac{\tilde\rho_v}{\varepsilon}\\
\nabla\times\widetilde{E}&=-j\omega\mu\widetilde{H}\\
\nabla\cdot\widetilde{H}&=0\\
\nabla\times\widetilde{H}&=\widetilde{J}+j\omega\varepsilon\widetilde{E}
\end{align*}$$
where
- $\widetilde{E}$ = [[Time]] varying electric field

 [[Current Density]] can be written interms of complex permittivity, and the [[Triple Product#Scalar Triple Product|Scalar Triple Product]] of any vector field is zero. Therefore the equations become:
$$\begin{align*}
\nabla\cdot\widetilde{E}&=0\\
\nabla\times\widetilde{E}&=-j\omega\mu\widetilde{H}\\
\nabla\cdot\widetilde{H}&=0\\
\nabla\times\widetilde{H}&=j\omega\varepsilon_c\widetilde{E}
\end{align*}$$
where
- $\varepsilon_c$ = [[Permittivity#Complex Permittivity|Complex Permittivity]]

>[!note]
>The above equations are given in the frequency domain

---

#### The Wave Equation
From these equations, the following can be derived:
$$\begin{align*}
\frac{\partial^2E}{\partial x^2}&=\mu_0\varepsilon_0\frac{\partial^2E}{\partial t^2}\\
\frac{\partial^2B}{\partial x^2}&=\mu_0\varepsilon_0\frac{\partial^2B}{\partial t^2}\\
\therefore\frac{\partial B}{\partial x}&=-\mu_0\varepsilon_0\frac{\partial E}{\partial t}
\end{align*}$$


This equation is similar to that used to caluclate [[Speed of Light]], and a relation does exist:
$$
c=\frac 1{\sqrt{\mu_0\varepsilon_0}}
$$
It also follows that:
$$
\frac {E_{max}}{B_{max}}=c
$$
This is the connection between the [[Electric Field]], [[Magnetic Field]], and the [[Electromagnetic Wave]]



