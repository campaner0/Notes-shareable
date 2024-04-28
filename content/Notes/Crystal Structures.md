---
type: note
---
02/05/2024 18:13

Tags: #Chemistry #Materials_Science 

allotropes - same material, different crystal structures

## Unit cells
- Simplest repeating unit in crystal
	- Many diff cell shapes possible
	- Smallest cell representing best symmetry chosen
- Primitive
	- All atoms (lattice points) at corners
- Non-primitive
	- All lattice points not at corners, possible to have some inside

## Bravais Lattices
- 7 crystal systems
- 14 Bravais lattices
- Cubic $a=b=c$;  $\alpha=\beta=\gamma=90^\circ$
	- Primitive
		- Simple cubic
	- Non-primitive
		- Face-centered (FCC)
		- Body-centered (BCC)
- Tetragonal $a=b\ne c$;  $\alpha=\beta=\gamma=90^\circ$ 
	- P
		- Simple tetragon
	- N-p
		- BCC
		- Hexagonal
- Hexagonal $a=b\ne c$;  $\alpha=\beta=90^\circ$;  $\gamma=120^\circ$  
- Orthorhombic  $a\ne b\ne c$;  $\alpha=\beta=\gamma=90^\circ$ 
- Monoclinic  $a\ne b\ne c$;  $\alpha\ne 90^\circ$;  $\beta=\gamma=90^\circ$ 
- Rhombohedral $a=b=c$;  $\alpha\ne\beta\ne\gamma\ne90^\circ$ 
- Triclinic $a\ne b\ne c$;  $\alpha\ne\beta\ne\gamma\ne90^\circ$ 

Simple cubic crystal structure 
- Atoms are touching, but do not overlap
$$\begin{align*}
\text{Atomic Packing Fraction}&= \frac{\frac{4}{3}\pi r^3}{a^{3}}\\
&= 0.5236
\end{align*}$$
where
- $r=a/2$

BCC

$$\begin{align*}
\text{APF}&= \frac{\frac{8}{3}\pi r^3}{a^{3}}\\[5pt]
&= \frac{\sqrt{3}}{8}\pi=0.6802
\end{align*}$$
where
- $r=\frac{\sqrt{3}}{4}a$

FCC

$$
\begin{align*}
\text{APF}&= \frac{\frac{16}{3}\pi r^3}{a^{3}}\\[5pt]
&= \frac{1}{3\sqrt{2}}\pi=0.7405
\end{align*}
$$
where
- $r=\frac{a}{2\sqrt{2}}$

Diamond and Zinc Blende structure
- Two merged FCC lattices offset by a/4 in x, y, z directions
	- Diamond crystalizes in same structure (namesake)
	- Inside atoms in tetrahedral structure
		- In binary semi, each atom bonded to 4 of other element
	- if two elements in this structure: zinc blende 


---

## Volume Density

For cubic structure:

$$
\rho_{v}=\frac{nM}{a^{3}N_{a}}
$$
where
- $n$ = number of atoms in cube
- $M$ = [[Atomic Weight]] of material
- $a$ = lattice constant
- $N_a$ = [[Mole|Avogadro's number]]

---

## Miller Indices
- Electronic properties diff on diff cuts of material
- Miller Indices - 3 integers with no common factors, written (abc)
	- Inversely proportional to intercepts of crystal plane along three axes
	- Determines orientation of slice
	- Negative numbers written with line over number ex. $(1\bar{1}2)$
	- Parallel to axis, intercept written as ∞
	- If plane intersects origin, choose new origin
		- Choose new if axis not intersected in box
1. Find intercepts of plane on axes
2. Take reciprocal of intercepts
3. Reduce to smallest integer value (multiply by lcd)
4. Enclose in parentheses
$$\begin{align*}
& \begin{array}{c|c|c|c}
& x & y & z\\
\hline
\text{Intercepts} & 2 & 3 & 2\\
\text{Reciprocals} & \frac{1}{2} & \frac{1}{3} & \frac{1}{2} \\
\text{Multiply by LCD} & 3 & 2 & 3\\
\text{Reduce} & 3 & 2 & 3
\end{array}\\\\
\\
& \text{Result} = (323)
\end{align*}$$

- Directions
	- Written as \[u v w]
		- Integers represent coordinates of vector
		- One index for start (tail) and one for end (head) of vector
	- To find direction, subtract tail from head, then multiply by lcd
- Silicon wafers
	- Flat wafers cut out of cylindrical ingot
	- (110) and (111) most widely used planes to cut wafers