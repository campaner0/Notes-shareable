---
type: note
aliases:
  - Consistency
  - Consistent
---
09/14/2022 10:40

  #Linear_Algebra 

In linear algebra, a system of equations may be consistent or inconsistent.

It is consistent if there is:
1. A unique solution
2. Infinitely many solutions

It is inconsistent if there is no solution


>[!note]
>The consistency of a system can be evaluated if its matrix is at least in [[Echelon Form]]. If there are pivots in every row, the system is consistent. If there are not pivots in every row, the system may or may not be consistent


### Examples
$$
\begin{bmatrix}1&3&-3 \\ 0&h-3&12\end{bmatrix}
$$
This system is consistent only when $h\neq 3$. If $h=3$, then the second row would result in the following equation, which is false:
$$
0\cdot x_{1}+0\cdot x_{2}=12
$$
For any other $h$, the system has a unique solution.

---
$$
\begin{bmatrix}1&3&-9 \\ 0&h-3&0\end{bmatrix}
$$
This system is consistent for all $h$, ($h\in \mathbb{R}$). If $h=3$, then $x_2$ is free and the system has infinitly many solutions. If $h\neq 3$, the system has a unique solution.