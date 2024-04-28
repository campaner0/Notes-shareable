---
type: note
tags: [Physics]
---
04/19/2022 13:06

  

Ampere's Law states that the contour integral of the [[Magnetic Field]] around a loop is equal to the total current as the sum of real and displacement current within the Amperian loop, if current is constant. This is given by:
$$
\oint_C\vec{H}\cdot d\vec{\ell}=I+I_{d}\tag{1}\label{1}
$$
where
- $I$ = [[Current]]
- $I_d$ = [[Displacement Current]]
- $\vec{H}$ = [[Magnetic Field Strength]]


### Differential form:
$$
\nabla\times\vec{H}=\vec{J}\tag{2}
$$
where
- $\vec{J}$ = [[Current Density]]

>[!note]
>This is another way of stating the [[Biot-Savart Law]].

---

### Special Cases
If the radius $r$ of the Amperian loop is smaller than the circumference of a wire $R$ that passes through it, the current flowing inside the loop $I'$ is given by:
$$
I'=\frac{r^2}{R^2}I
$$
where
- $I$ = total current in wire
- $r$ = radius of Amperian loop
- $R$ = radius of conductor

Replacing $I$ with $I'$ in $\eqref{1}$:
$$
B=\frac{\mu_0r}{2\pi{R^2}}I
$$
If $r\ge R$:
$$
B=\frac{I}{2\pi r}
$$


>[!note]
>For a toroid, where the wire is coiled around a ring, the current flowing through an Amperian loop in the same space as the ring is $NI$, where N is the number of turns of wire.

