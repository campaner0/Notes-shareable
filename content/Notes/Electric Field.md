---
type: note
---
03/20/2022 18:03

Tags: #Physics 

The Electric field in an area is a [[Vector Field]] of the [[Force]]s that an infinitesimal positive test [[Charge]] would experience at each point in that area. Hence:
$$
\vec E= \frac{\vec F_e}{q_0}
$$
where
- $\vec{E}$ = electric field vector (V/m or N/C)
- $\vec{F_e}$ = [[Electromagnetic Force#Electric Force|Electric Force]] felt by a charge
- $q_0$ = charge experiencing the force

It also follows that $\vec{E}\equiv\vec{F_e}$ if test charge is infinitesimal


#### Field created by a point charge:
$$
\vec{E}=k_e\frac{q}{r^2}\hat{r}
$$
Where 
- $k_e$ = Coulomb's Constant $(\frac{1}{4\pi\varepsilon_0})$ 
- $q$ = [[Charge]]
- $r$ = distance from charge to measurement point (m)
- $\hat{r}$ = [[Unit Vector]]

---

#### Field created by multiple charges:
$$
\vec{E}=k_e\sum_i{\frac{q_i}{r^2_i}}\hat{r}
$$
- Sum of fields created by all charges at that point

---

#### Potential
Electric field can be calculated as the [[Gradient]] of electric potential (with the [[Magnetic Vector Potential]] term when time-varying):
$$
\vec{E}=-\nabla V-\frac{\partial\vec{A}}{\partial t}
$$
where
- $V$ = [[Voltage]]
- $\vec{A}$ = [[Magnetic Vector Potential]]

---

#### Motion of charge in E field
$\vec{F}=q\vec{E}=m\vec{a}$ by [[Newton's Second Law]], so
$$
\vec{a}=\frac{q\vec{E}}{m}
$$
therefore
$$
v_p=\sqrt{\frac{2qEd}{m}}
$$
where
- $v_p$ = [[Velocity]] of particle
- $q$ = [[Charge]]
- $E$ = magnitude of electric field
- $d$ = distance traveled ($x-x_i$)
- $m$ = [[Mass]] of particle

---

#### Connection to Magnetic Field
Since [[Voltage]] is the integral of the electric field and voltage is the derivative of [[Magnetic Flux]], this relationship is revealed:
$$
\int\vec{E}\cdot d\vec{s}=-\frac{d\Phi_B}{dt}
$$
