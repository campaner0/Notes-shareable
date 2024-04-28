---
type: note
alias: Magnetic Circuits
tags: [Circuit_Analysis]
---
10/10/2022 16:18

  

A magnetically coupled circuit is a circuit that uses [[Inductance#Mutual Inductance|Mutual Inductance]] to create a complete circuit. Magnetic circuits model the behavior of magnetic flux through a closed loop. Similarly to how a [[Voltage]] source induces [[Current]] in an electric circuit, the current through a coil induces a flux through a magnetic core, and another coil may resist the flux created by the first. Therefore, it is possible to draw a magnetic circuit in the same way an electric circuit is drawn, even using the same symbols. A [[Transformer]] is a common usecase. 


### Energy 
For any magnetically coupled circuit, the [[Energy]] stored in the circuit at a [[Time]] $t$ is:
$$
w(t)=\frac{1}{2}L_1({i_1}^2)+\frac{1}{2}L_2({i_2}^2)\pm M(i_1)(i_2)
$$
where
- $L_n$ = [[Inductance]] of nth inductor
- $i_n$ = [[Current]] through nth inductor
- $M$ = mutual inductance of system


Since energy cannot be negative, the following relation must be true:
$$
M\le\sqrt{L_1L_2}
$$

---

### Coupling Coeffiecient
The closer the circuit is to ideal, that is, to unity of the coils, the closer $M$ will be to $\sqrt{L_1L_2}$. This is reflected in the coupling coeffiecient:
$$
k=\frac{M}{\sqrt{L_1L_2}}
$$
where
- $0\le k\le 1$

The closer $k$ is to 1, the more ideal the circuit. For the ideal case, see [[Transformer#Ideal Transformer|Ideal Transformer]]