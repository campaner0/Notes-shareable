---
type: note
aliases:
  - Lorentz Force
  - Electric Force
  - Magnetic Force
---
03/22/2022 23:01

  #Physics 

One of [[The Four Fundamental Interactions]]. Describes the forces surrounding electric charge and magnetism. It is the sum of electric and magnetic forces:
$$
\vec{F}=q(\vec{E}+\vec{v}\times\vec{B})
$$

### Electric Force
Coulomb's Law states that the [[Force]] experienced by two charges is the ratio of the product of the two charges' magnitudes and the square of the distance between them, all multiplied by a constant:
$$
\vec{F_e}=k_e\frac{q_1q_2}{r^2}\hat{r}
$$
where
- $k_e$ = Coulomb's constant ($\frac1{4\pi{\varepsilon_0}}$ or $8.9876\times 10^9$ $\text{Nm}^2/\text{C}^2$)
- $q_n$ = magnitude of [[Charge]] n (C)
- $r$ = distance between (m)
- $\hat r$ = unit vector

The electric force a particle experiences is also equal to the product of the charge and the [[Electric Field]] at its location:
$$
\vec{F_e}=q_0\vec{E}
$$

---

### Magnetic Force
Mag force on a particle depends on the [[Velocity]] of the particle
$$
\vec{F_B}=q\vec{v}\times\vec{B}
$$
where
- $\vec{B}$ = [[Magnetic Field]] vector
- $\vec{v}$ = velocity vector

>[!note]
>Due to the rules of the [[Cross Product]], the force on the particle will be perpendicular to velocity and mag field, resulting in [[Circular Motion]] of the particle when in a uniform magnetic field.

According to [[Newton's Second Law]], the rules of the cross product, and rules of circular motion, $\vec{F_B}=ma_c$, $\left|\vec{F_B}\right|=qvB\sin{\theta}$, and $a_c=\frac{v^2}{r}$, therefore:
$$
r=\frac{mv}{qB}
$$
$$
T=\frac{2\pi{m}}{qB}=\frac{2\pi{r}}{v}
$$
$$
\omega=\frac vr=\frac{qB}m
$$
where
- $r$ = radius of motion
- $T$ = period
- $\omega$ = [[Angular Velocity|Angular Frequency]]


#### Magnetic Force on a Conductor
If [[Current]] flows through conductor in a mag field, it will experience mag force described by:
$$
\vec{F_B}=I\vec{L}\times\vec{B}
$$
where
- $I$ = current through conductor
- $\vec{L}$ = length [[Vector]] of wire

>[!note]
>In a uniform mag field, the net force on a wire of any shape is 0

##### Magnetic Force Between Two Parallel Conductors
If the currents in the wires are flowing in the same direction, the force on both will be toward each other. If opposite, wires will repel.

Force per unit length is given by:
$$
\frac{\vec{F_B}}{\ell}=\frac{\mu_0I_1I_2}{2\pi a}
$$
where
- $\ell$ = length of wire
- $a$ = distance between wires
- $I$ = current in each wire respectivly