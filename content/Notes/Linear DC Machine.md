---
type: note
---
01/24/2023 18:37

Tags: #Electric_Machines 

The linear DC machine operates based on the principle of the [[Electromagnetic Force#Magnetic Force on a Conductor|Magnetic Force on a Wire]] when current flows through it:

![[Pasted image 20230124183829.png]]

If a bar is placed on frictionless rails in a static magnetic field, when the switch is closed and current flows, the bar  experiences an induced force. When it starts to move, an opposite force opposes the movement of the bar due to [[Motional EMF]]. Changing the direction of applied current flow changes the direction of movement of the bar.

The electrical power converted to mechanical form (assuming no losses) is given by:
$$
P=F_{ind}v
$$
where
- $P$ = electrical [[Electrical Power]]
- $F_{ind}=ilB$ = induced [[Force]]
- $v$ = [[Velocity]] of bar

## As a Motor
The machine acts as a motor when $\varepsilon_{ind}<V_B$ and the applied force is opposite to the direction of motion. In this case, current is described by:
$$
i= \frac{V_{B}-\varepsilon_{ind}}{R}
$$
where
- $i$ = [[Current]]
- $V_B$ = applied [[Voltage]]
- $\varepsilon_{ind}$ = induced emf
- $R$ = [[Resistance]]

>[!note]
>In this machine, whether it is acting as a generator or motor, the bar moves in the same direction.

---

## As a Generator
If a force is applied in the same direction as the motion of the bar, the velocity increases until $\varepsilon_{ind}>V_B$. At this point, the current is described by:
$$
i= \frac{\varepsilon_{ind}-V_{B}}{R}
$$


