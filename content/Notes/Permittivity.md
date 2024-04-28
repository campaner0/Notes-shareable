---
type: note
tags: [Physics, Electromagnetics, Semiconductor_Devices]
---
10/25/2022 17:57

  

Permittivity is a measure of how easily a material polarizes. High permittivity means a material will polarize more when exposed to an electric field than a material with low permittivity. The permittivity of a material is the product of vacuum permittivity and its relative permittivity. (Units: $F/m$)
$$
\varepsilon=\varepsilon_0\varepsilon_r
$$
where
- $\varepsilon_0$ = Vacuum Permittivity
- $\varepsilon_r=1+\chi$ = relative permittivity
	- where $\chi$ = [[Electric Susceptibility]]

### Vacuum Permittivity
The permittivity of free space is an electric field's ability to permeate a vacuum. It is defined by:
$$
\begin{align*}
\varepsilon_{0} &= \frac{1}{c^2\mu_0}\\[5pt]
&= 8.85418782 \times 10^{-12}\,\text{F/m}
\end{align*}
$$
where
- $c$ = [[Speed of Light]]
- $\mu_0$= Vacuum [[Permeability]]

Vacuum permittivity is used in defining [[Electromagnetic Force#Electric Force|Electric Force]] and the [[Electric Displacement Field]].

---

### Complex Permittivity
The permittivity of a dielectric generally depends on the frequency of the field, and, since there is a phase difference between the electric field and polarization, permittivity must be a [[Complex Numbers|Complex Number]] to account for this:
$$\begin{align*}
\varepsilon_c&=\varepsilon-j \frac{\sigma}{\omega}\\
&=\varepsilon'+\varepsilon''
\end{align*}$$
where
- $\varepsilon_c$ = complex permittivity
- $\varepsilon$ = real part 
- $\sigma$ = [[Conductivity]] of medium
- $\omega$ = [[Angular Velocity|Angular Frequency]] of applied [[Electric Field]]
