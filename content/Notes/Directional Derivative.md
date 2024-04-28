---
type: note
---
08/23/2022 18:05

Tags: #math 

The directional [[Derivative]] of a scalar function along a [[Vector]] is the [[Dot Product]] of the function's [[Gradient]] and the [[Unit Vector]] in the direction of the vector:
$$
D_{\vec u}f=\vec\nabla f\cdot\vec{u}
$$
where
- $f$ is a scalar function
- $\vec{u}$ = unit vector


### Rate of Change
Using the dot product identity, this can be written as
$$\vec\nabla f\cdot\vec u=|\vec\nabla f|\cos\theta=
	\begin{cases}
	|\vec\nabla f|, & \text{if $\theta=0$ (max rate of change)} \\
	-|\vec\nabla f|, & \text{if $\theta=\pi$ (min rate of change)} \\
	|\vec\nabla f|, & \text{if $\theta=\frac{\pi}{2}$(no rate of change)} \\
	\end{cases}$$
where
- $\theta$ = 