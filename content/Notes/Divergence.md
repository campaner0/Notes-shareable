---
type: note
---
08/18/2022 18:14

Tags: #math #Physics 

Divergence is a measure of the [[Flux]] density through a volume, or the flux per unit [[Volume]] over a closed surface. It is denoted as:
$$
\nabla\cdot\vec{V}= \frac{\partial\vec{V}}{\partial x}+\frac{\partial\vec{V}}{\partial y}+\frac{\partial\vec{V}}{\partial z}
$$
where
- $\vec V$ = [[Vector Field]]

>[!note]
>The divergence of a vector field is a scalar

---

### Divergence Theorem

The divergence theorem relates the volume integral of the divergence to the flux of the vector field through the volume:
$$
\int_V\nabla\cdot\vec{E}\,dV=\oint_S\vec{E}\cdot d\vec{s}
$$
where
- $\vec{E}$ = vector field
- $\vec{E}\cdot d\vec{s}$ = $\vec{E}\cdot\hat{n}\,ds$ 
	- where $\hat{n}$ = [[Normal Vector]] to surface