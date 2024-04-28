---
type: note
alias: Induction Motors
tags: [Electric_Machines]
---
03/21/2023 18:54

  

The stator of the induction motor is similar to an [[AC Motors|AC Motor]] (synchronous), but the rotor is different. It can be a squirrel cage rotor or wound rotor. The squirrel cage motor does not need brushes, while the wound rotor does.


Similarly to a sychronous motor, the induction motor is powered by three phases which create a rotating magnetic field. The speed of the field rotation in given by:
$$
n_{sync}=\frac{120f_{se}}{P}
$$
where
- $n$ = speed of [[Magnetic Field]] rotation
- $f_{se}$ = electrical [[Frequency]]
- $P$ = number of poles

Rotor frequency:
$$\begin{align*}
f_{re}&= sf_{se}\\[5pt]
&= \frac{P}{120}(n_{sync}-n_m)
\end{align*}$$
where
- $f_{re}$ = rotor frequency
- $s=\frac{(n_{sync}-n_m)}{n_{m}}$ = slip
- $n_m$ = mecanical shaft speed

>[!note]
>Slip can be expressed as a percentage by multiplying by 100

### Power

![[Pasted image 20230330183348.png]]
$$\begin{align*}
P_{SCL}&= 3I^2_1R_1\\[5pt]
P_{core}&= 3E^2_1G_C\\[5pt]
P_{AG}&= \frac{3I^{2}_{2}R_{2}}{s}\\[5pt]
&= \tau_{ind}\omega_{sync}\\[5pt]
P_{RCL}&= 3I^{2}_{2}R_{2}\\[5pt]
&= 3I^{2}_RR_{R}\\[5pt]
&= sP_{AG}\\[5pt]
P_{conv}&= (1-s)P_{AG}\\
&= \tau_{ind}\omega_m
\end{align*}$$


----
### Torque
The total induced torque in the machine when rotating counterclockwise is given by:
$$
\tau=k\vec B_r\times\vec B_s
$$
where
- $\tau$ = [[Torque]]
- $k$ = 
- $\vec B_r$ = magnetic field produced by current in rotor
- $\vec B_s$ = magnetic field due to current in stator

---

### Losses
The losses in an induction motor are similar to those in a [[Transformer]] since they share characteristics like a core, windings, etc, but they are not totally the same. An induction motor has:
- stator copper losses
- core losses
Air gap power
- rotor copper
- friction and windage
- stray

The air gap above is the gap between the rotor and stator. The losses above the air gap occur on the stator side, and the others on the rotor side.