---
type: note
tags: [Physics, Circuit_Analysis]
---
03/21/2022 17:11

  

Inductance is the tendency of a conductor to oppose a change in current flowing through it. This is the idea behind [[Magnetic Flux#Lenz's Law|Lenz's Law]]: current flow cannot change instantaneously. This is described by:
$$
V_L=L\frac{di}{dt}
$$
Inductance of a conductor can be found by the ratio of its magnetic field and current:
$$
L=\frac{N\Phi_B}{I}
$$
where
- $L$ = inductance
- $N$ = number of turns in inductor (if applicable)
- $\Phi_B$ = [[Magnetic Flux]]
- $I$ = [[Current]]

#### Inductance of a Coil
Using the above equation that relates inductance to mag flux, inductance can be described by:
$$
L=\frac{\mu N^2A}{\ell}
$$
where 
- $\mu$ = [[Permeability]] of core
- $A$ = cross-sectionsl [[Area]] of coil

Mag flux is described by the product of mag field and area, and mag field by [[Ampere's Law]]

---

#### Mutual Inductance
Mutual inductance is when one coil's mag field induces a current in another coil.
$$
M_{12}=\frac{N_2\Phi_{12}}{i_1}
$$
where
- $M$ = mutual inductance

The two coils then induce an emf in each other such that the voltage in one is the negative of the other's. The secondary coil's voltage is given by:
$$
V_2(t)=M_{21}\frac{di_1}{dt}+L_2\frac{di_2}{dt}
$$
where
- $M_{21}$ = Mutually induced inductance in secondary coil due to primary
- $L_2$ = inductance of secondary coil

