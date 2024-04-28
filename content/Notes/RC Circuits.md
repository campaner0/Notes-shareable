---
type: note
---
03/21/2022 14:46

  #Circuit_Analysis, #Physics 

Circuit made up of only resistors and capacitors (and possibly source). These can be reduced to an equivalent circuit with one cap ($C_{eq}$) and one resistor ($R_{eq}$)

Voltage across cap cannot change instantaneously, but current can. Described by:
$$
i_c=C\frac{dv}{dt}
$$
where
- $i_c$ = [[Current]] through cap
- $C$ = [[Capacitance]]
- $v$ = [[Voltage]] across cap
- $t$ = [[Time]]

#### Source Free RC Circuits
This scenario happens when capacitor is charged and then source is disconnected
Solving the above differential equation, voltage at a time t is given by
$$
v(t)=V_0exp\left(\frac{-t}{\tau}\right)
$$

#### Driven RC Circuit
RC circuit with switched source. Area of interest: transient behavior between switch closed/opened and o.p.

##### Charging Capacitor
Solving the above differential equation, transient voltage accross the capacitor as it charges is described by:
$$
v(t)=V_0\left(1-exp\left[\frac{-t}{\tau}\right]\right)
$$
where
- $V_0$ = source voltage
- $\tau=RC$ ([[Time Constant]])

Using $Q=C\Delta V$, the voltage equation can be adapted to show charge on cap over time: $q(t)=Q_{max}\left(1-exp\left[\frac{-t}{\tau}\right]\right)$
Since current does not flow when the cap is charged, it must peak when switch is closed

##### Discharging Capacitor
For discharging, the equation is the same as a source free circuit

A cap is fully charged/discharged after 5$\tau$

##### RC Circuit with Step 
The equation is the same as an RL circuit, but with voltage and current switched:
![[RL Circuits#RL Circuit with Step]] 




