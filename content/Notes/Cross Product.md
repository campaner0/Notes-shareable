---
type: note
tags: [Math]
---
03/25/2022 18:17

 

The cross product of two [[Vector]]s is the [[Determinant]] of a matrix in which the first row is populated by the standard unit vectors of the chosen coordinate system, and the second and third row by the values of each vector. In $\mathbb R^3$ with cartesian coordinates:
$$
\vec{v}\times\vec{u} =
	\left|\begin{matrix}
	\hat{i} & \hat{j} & \hat{k} \\
	v_1 & v_2 & v_3 \\
	u_1 & u_2 & u_3 \\
	\end{matrix}\right| \\
$$
The result is a vector which is [[Orthogonal]] to both $\vec v$ and $\vec u$. If the angle between the vectors is known, the cross product can be found using the following relation:
$$
\vec{v}\times\vec{u}=(|\vec v||\vec u|\sin\theta)\hat n
$$
where
- $\theta$ = [[Angle]] between the vectors
- $\hat n$ = unit [[Normal Vector]] which is normal to the plane that contains both vectors

---

### Properties

>[!info] Algebraic Properties
> - if $\vec{v}\times\vec{u} = \vec 0$, $\vec v$ and $\vec u$ are parallel $\forall\,\, \vec{v},\vec{u}\ne\vec 0$
> - $\vec{v}\times\vec{u}=-(\vec{u}\times\vec{v})$
> - $a(\vec{v}\times\vec{u})=(a\vec{v})\times\vec{u}=\vec{v}\times(a\vec{u})$
> - $\vec{w}\times(\vec{v}+\vec{u})=(\vec{w}\times\vec{v})+(\vec{w}\times\vec{u})$
> - $|\vec{v}\times\vec{u}|^2=|\vec v|^2|\vec u|^2-(\vec{v}\cdot\vec{u})^2$

>[!info] Geometric Properties
> - $\vec{v}\times\vec{u}\perp\vec{v},\vec{u}$
> - $\vec{v}\times\vec{u}$ is the area of a parallelogram with $\vec v$ and $\vec u$ as adjacent sides
