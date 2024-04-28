---
type: note
---
04/07/2022 12:49

  #Physics 

Faraday's Law describes how changing magnetic field can induce an [[Voltage|Electromotive Force]]:
$$
V_{emf}=-N\frac{d\Phi_B}{dt}
$$
where
- $V_{emf}=V_{emf}^{tr}+V_{emf}^m$ 
	- $V_{emf}^{tr}$ = [[Transformer EMF]]
	- $V_{emf}^m$ = [[Motional EMF]]
- $N$ = number of turns of coil
- $\Phi_B$ = [[Magnetic Flux]]
- $t$ = [[Time]]

>[!note]
>For a loop that is fixed in space, an [[Electric Field]] is created if mag field varies since [[Voltage]] is the integral of electric field.

Combining with the magnetic flux equation:
$$
\left|\varepsilon\right|=\frac{d(BA)}{dt}
$$
for a single turn.

For a square loop:
$$
\left|\varepsilon\right|=B\ell v
$$
since [[Velocity]] is the derivative of position. In this case, x is the [[Position]] of one side of a square loop which can move without breaking the circuit, changing the size of the loop. The resulting velocity is the rate of change of the width of the loop.

If we apply [[Ohm's Law]]:
$$
I=\frac{B\ell v}{R}
$$
where
- $I$ = [[Current]]
- $R$ = [[Resistance]]

Then applying the formula for [[Electromagnetic Force#Magnetic Force on a Conductor|Magnetic Force]]:
$$
F_B=\frac{B^2\ell^2v}{R}
$$
This is the magnetic force opposing the change in the size of the loop, which is equal to the applied force if the loop is changing size.

Applied [[Electrical Power]] can be found by applying the formula $P=I^2R$:
$$
P=(B\ell v)^2=F_Bv
$$
