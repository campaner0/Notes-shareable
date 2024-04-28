---
type: note
tags: [Circuit_Analysis, Physics]
---
03/21/2022 14:46

 , 

Circuit made up of only resistors and inductors (and source)
These can be reduced to an equivalent circuit with one inductor ($I_{eq}$) and one resistor ($R_{eq}$)

Current through an inductor cannot change instantaneously, but voltage can. Described by:
$$
v_l=L\frac{di}{dt}
$$
where
- $v_l$ = [[Voltage]] across inductor
- $L$ = [[Inductance]]
- $i$ = [[Current]]

### Source Free RL Circuits
This scenario happens when inductor is charged and then source is disconnected
Solving the above differential equation, current at a [[Time]] t is given by:
$$
i(t)=I_0exp\left(\frac{-t}{\tau}\right)
$$
where
- $I_0$ = source current
- $\tau=\frac{L}{R}$ ([[Time Constant]])

Similarly for voltage across the resistor:
	$$
v_r=V_0exp\left(\frac{-t}{\tau}\right)
$$
where
- $v_r$ = voltage across a parallel resistor (same as voltage across inductor)
- $V_0$ = source voltage

For voltage across inductor, use above differential equation

---

### Driven RL Circuits
Area of intrest: transient behavior with sudden application of dc source (switch)

#### Charging Inductor
##### Current
- Inductor acts as short at $t(0^-)$, so $I=\frac{V}{R}$ at operating point
therefore, by solving above diff eq:
$$
i(t)=\frac{V_0}{R}\left(1-exp\left[\frac{-t}{\tau}\right]\right)
$$
where
- $V_0$ = constant source voltage

More generally, this is the sum of forced and natural responses, forced being the current through the circuit at $t=\infty$. Given by
$$
f(t)=f(\infty)+Aexp\left(\frac{-t}{\tau}\right)
$$
##### Voltage
Plugging in the source free formula for current into the differential equation gives a formula for voltage across the inductor over time:
$$
v(t)=RI_0exp\left(\frac{-t}{\tau}\right)
$$


#### Discharging Inductor
Equation is negative:
$$
i(t)=-\frac{V_0}{R}\left(1-exp\left[\frac{-t}{\tau}\right]\right)
$$

An inductor is fully (dis)charged after 5$\tau$

##### RL Circuit with Step
Driven circuit but an unswitched source and switched source
- switched source is essentially a source with its magnitude multiplied by the [[Step Function]] u(t)
therefore
$$
i(t)=\frac{V_0}{R}+\frac{V_s}{R}\left(1-exp\left[\frac{-t}{\tau}\right]\right)u(t)
$$
where
- $V_s$ = switched source voltage
- $u(t)$ = step function

---

#### Energy Stored in a Magnetic Field
The [[Electrical Power]] absorbed by an inductor can be found through the usual power equation, where voltage is replaced with the inductor voltage:
$$
P=\varepsilon L\frac{di}{dt}
$$
