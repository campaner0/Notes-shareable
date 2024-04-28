---
type: note
tags: [Electric_Machines]
---
04/11/2023 18:35

  

DC electric machines recieve/produce a DC current instead of an [[Alternating Current|AC]] current. The armature refers to the rotor of the machine, and the field current is through the stator, which is the opposite of AC machines.

## Windings

### Wave
armature coils connected s.t. there are two parallel routes
$$
a = 2m
$$
where
- $a$ = number of current paths
- $m$ = plex of motor

---

### Lap
coils connected s.t. # of parallel paths = # of poles. better for big machines (more paths = more current)

$$
a=mP
$$
where
- $P$  = number of poles

---

## Internal Voltage/Torque

$$
E_A=k\Phi\omega_m
$$
where
- $k= \frac{ZP}{2\pi a}$
	- $Z$ = number of conductors on rotor
- $\Phi$ = [[Magnetic Flux]] per pole

$$\begin{align*}
\tau&= k\Phi I_A\\
&= kcI_A^2
\end{align*}$$
where
- $I_A$ = armature [[Current]]

---

## Losses
DC machines have the same losses as AC machines: copper, core, mechanical, and stray losses, but they also have losses from the brushes. These are due to the voltage drop where the brushes contact the armature:
$$
P_{BD} = V_{BD}I_A
$$
where
- $P_{BD}$ = brush [[Electrical Power|Power]] loss
- $V_{BD}$ = brush [[Voltage]] drop
- $I_A$ = armature current

---

## Types of Motors
DC motors can be categorized by how their armature and field circuits are connected. See [[DC Motor Equivalent Circuit]] 