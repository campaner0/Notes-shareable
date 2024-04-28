---
type: note
alias: Transformers
---
10/11/2022 18:09

Tags: #Circuit_Analysis #Electromagnetics #Electric_Machines 

A transformer uses a magnetic field to change the amplitude of the [[Voltage]] of an input signal without affecting [[Frequency]]. It is made up of two or more coils of wire and a magnetic core. This core asists in directing the [[Magnetic Flux]] from one coil to the other, which completes the circuit without an electrical conection between the windings. The [[Electrical Power]] is kept constant through this transformation, therefore if the voltage is raised, the [[Current]] must drop and vice versa. 


### Reflected Impedance 
Given:
![[Pasted image 20221012163706.png]]

The impedance seen by the source due to the the primary loop and the secondary loop is: 
$$
Z_{in}=Z_{1}-\frac{(j\omega)^2M^2}{Z_{2}}
$$
where
- $Z_{1}$ = [[Impedance]] of first coil
- $Z_{2}$ = impedance of second coil
- $M$ = [[Inductance#Mutual Inductance|Mutual Inductance]]
- $\omega$ = [[Angular Velocity|Angular Frequency]] of source

---

### Ideal Transformer
For an ideal transformer, where $k=1$ (see [[Magnetically Coupled Circuits#Coupling Coeffiecient|Coupling Coeffiecient]]):
$$
\begin{align*}
\frac{V_1}{V_2}&= \frac{N_1}{N_2}=a\\[5pt]
\frac{I_1}{I_2}&= \frac{1}{a}\\[5pt]
V_1I_{1}&= V_2I_2\\[5pt]
\frac{L_2}{L_1}&=\left( \frac{1}{a}\right)^2
\end{align*}
$$
where
- $V_1$ = primary coil [[Voltage]]
- $I_1$ = primary coil [[Current]]
- $L_1$ = primary coil [[Inductance]]

Manipulating these equations and applying [[Ohm's Law]], the following relation emerges:
$$
Z_{in}=a^2(Z_L)
$$
where
- $Z_{in}$ = [[Impedance]] of input
- $Z_L$ = impedance of load

>[!info]
>These relations hold true for phasor values as well as magnitudes

#### Magnetic Field in Transformer
A coil in an ideal transformer with current $i$ and length of core $l_c$ will produce a magnetic field of:
$$
H=\frac{Ni}{l_c}
$$
where $H$ = [[Magnetic Field Strength]]. This comes from a simplification of [[Ampere's Law]]. 

---

### Non-ideal Transformers
In the real world, transformers are subject to losses, both electrical and magnetic. The effect of these losses is a higher current draw by the primary winding called excitation current:
$$
i_{ex}=i_m+i_{h+c}
$$
where
- $i_{ex}$ = excitation current
- $i_m$ = magnetization current
- $i_{h+c}$ = core loss current

#### Magnetization Current
Magnetization or magnetizing current is the current required to create magnetic flux in the core. It is a sort of start-up cost. This current flows in the primary winding even when the secondary is open. Due to its similarity to the way energy is stored in an inductor, this "loss" is often represented as a [[Reactance]].

#### Core-Loss Current
[[Magnetic Hysteresis]] and [[Eddy Current]]s also resist the flux in the core and manifests in the core-loss current. This current is nonlinear due to the nonlinear nature of hysteresis, but its fundamental component is in phase with the primary coil voltage.

#### Flux Leakage
Most of the flux produced by the primary winding travels through the core, but a small amount circles back to the primary through the air, bypassing the secondary. This also occurs at the secondary winding. In a well designed transformer:
$$\begin{align*}
\phi_M\gg\phi_{LP}\\
\phi_M\gg\phi_{LS}
\end{align*}$$
where
- $\phi_M$ = mutual flux
- $\phi_{LP}$ = leakage flux at primary

#### Copper (PR) Losses
Copper losses are due to the small resistances of the copper windings. This causes some energy to be lost to heat. It is proportional to the square of the current in the windings:

---

