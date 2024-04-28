---
type: note
---
05/10/2022 20:39

  #Statics 

Not to be confused with [[Moment of Inertia]]. Moment of inertia of areas, or second moment of area, or area moment of inertia, is a reflection of an object's stiffness and the stress it experiences due to an applied moment (or [[Torque]]). Units: $m^4$ or $in^4$ 

- Civil and mechanical engineering commonly refer to Second Moment as Moment of Inertia, while in physics, Moment of inertia refers strictly to the second moment of mass (the above linked moment of inertia).


Second moment of area is calculated with a [[Double Integral]]:
$$
I_x=\iint_R y^2dA
$$
$$
I_y=\iint_R x^2dA
$$
where:
- $I$ = second moment of area
- $x, y$ = distance to arbitrarily positioned axis

---

### Parallel Axis Theorem
If the shape is positioned with the rotational axis not at the [[Centroid]], the [[Parallel Axis Theorem]] may make the calculation easier. If $x$ passes through the centroid, and $x'$ is an arbitrary axis that does not pass through the centroid, the second moment about $x'$  is:
$$
I_{x'}=I_x+Ad^2
$$
where
- $A$ = Area of shape
- $d$ = distance from centroid to axis of rotation

---

### Perpendicular Axis Theorem
The second moment about an axis perpendicular to the plane of an area may be found by the sum of the moments about two axes parallel to the plane ([[Perpendicular Axis Theorem]]):
$$
J_z=\iint\rho^2dA=I_x+I_y
$$
where
- $J$ = second moment about perpendicular axis
- $\rho$ = radial distance from centroid to perpendicular axis