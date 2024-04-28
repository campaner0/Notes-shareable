---
type: note
alias: AC Motor
tags: [Electric_Machines]
---
02/23/2023 18:42

  



The relationship between mechanical speed of the rotor in revolutions per second and the electrical [[Frequency]] of the driving [[Current]] are related by a power of 2:
$$\begin{align*}
\theta_{se}&= \frac{P}{2}\theta_{sm}\\[5pt]
f_{se}&= \frac{P}{2}f_{sm}=\frac{n_{sm}P}{120}
\end{align*}$$
where
- $\theta_{se}$ = [[Angle]] of current
- $\theta_{sm}$ = angle of rotor
- $f$ = frequency
- $P$ = number of magnetic poles
- $n_{sm}$ = mechanical speed

## Induced Voltage
For a two pole machine, the induced voltage in the stator is:
$$
V_{ind}=N_C\Phi\omega\cos\omega t
$$
where
- $N_C$ = number of turns
- $\Phi$ = [[Magnetic Flux]]
- $\omega$ = [[Angular Velocity|Angular Frequency]]

>[!note]
>The RMS voltage is given as:
>$$
V_{A}=\sqrt{2}\pi N_{C}\Phi f
$$

---

## Induced Torque

$$\begin{align*}
\tau&= k\vec{B}_R\times\vec{B}_S\\[5pt]
&= kB_RB_{net}\sin\delta
\end{align*}$$
where
- $\vec{B}_R$ = rotor mag field
- $\vec{B}_S$ = stator mag field
- $\vec B_{net}=\vec B_R+\vec B_S$ 
- $\delta$ = 

>[!note]
>$k$ is often not constant since [[Permeability]] varies with magnetic saturation

