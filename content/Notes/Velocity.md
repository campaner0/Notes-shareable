---
type: note
---
03/20/2022 19:25

Tags: #Physics 

Velocity is a [[Vector]] defined by the rate of change of position with respect to time:
$$
\vec{v}=\frac{d\vec{r}}{dt}
$$
where
- $\vec v$ = velocity (m/s)
- $\vec{r}$ = [[Position]] (m)
- t = [[Time]] (s)

Similarly, the [[Derivative]] of velocity is [[Acceleration]]. Speed is the magnitude of velocity

#### With Constant Acceleration
$$
v_f=v_i+a\Delta t
$$
It is possible to express velocity independent of time:
$$
v_f^2=v_i^2+2a(x_f-x_i)
$$

---

#### Terminal Velocity/Freefall
Freefall equation:
$$
v(t)=\frac{mg}{b}\left(1-exp\left[-\frac{bt}{m}\right]\right)
$$
where
- $m$ = [[Mass]] (kg)
- $g$ = acceleration due to [[Gravity]] ($9.81m/s^2$)
- $b$ = resistance coefficient for the fluid (see [[Friction]])
- $t$ = time (s)

This describes the object's velocity over time. As the velocity approaches terminal velocity, the exponential term approaches 0, so terminal velocity is given by:
$$
v_t=\frac{mg}b
$$
##### Terminal Velocity in a Gas
When the fluid medium is a gas, terminal velocity is given by:
$$
v_t=\sqrt{\frac{2mg}{D\rho A}}
$$
where
- $m$ = mass (kg)
- $g$ = acceleration due to gravity
- $D$ = drag coefficient of gas
- $\rho$ = [[Density]] of gas ($kg/m^3$)
- $A$ = surface [[Area]] of object ($m^2$)

---

#### Escape Velocity
The velocity required to break free of a planet's gravity is escape velocity, defined by:
$$
v_e=\sqrt{\frac{2Gm_p}{r_p}}
$$
where
- $G$ = universal gravitational constant (see [[Gravity]])
- $m_p$ = mass of planet (kg)
- $r_p$ = distance from center of planet to object (m)