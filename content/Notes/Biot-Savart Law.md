---
type: note
---
11/12/2022 11:54

Tags: #Physics #Electromagnetics 

If current flows through a conductor, it will create a [[Magnetic Field]], which at a point near the wire is described by:
$$
\vec{B}=\frac{\mu_0I}{4\pi}\int\frac{d\vec{s}\times\hat{r}}{r^2}
$$
where
- $\mu_0$ = [[Permeability]]
- $\vec{s}$ = length [[Vector]] along wire
- $\hat{r}$ = [[Unit Vector]] in direction of point
- $r$ = distance from wire to point

---

### Calculations
For a finite length of wire, mag field at a point is given by
$$
B=\frac{\mu_0I}{4\pi{r}}(\sin{\theta_1}-\sin{\theta_2})
$$
where 
- $\theta_1$ = [[Angle]] of line from point to left end of wire (rad)
- $\theta_2$ = angle of line from point to right end of wire (neg rad)

For an infinite wire (in both directions), $\theta_1$ and $\theta_2$ approach (-)$\frac{\pi}{2}$, therfore:
$$
B=\frac{\mu_0I}{2\pi r}
$$

For a semi-infinite wire (in one direction), one angle approaches 0, the other (-)$\frac{\pi}{2}$ therefore:
$$
B=\frac{\mu_0I}{4\pi r}
$$

For a (circular) curved wire, starting from the original formula,
$s=r\theta$ so:
$$
B=\frac{\mu_0I}{4\pi r}\theta
$$