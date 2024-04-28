---
type: note
tags: [Linear_Algebra]
---
09/14/2022 11:33

  


In linear algebra, [[Matrix]]-[[Vector]] multiplication is given by:
$$
A\vec{x}=\begin{bmatrix}\vec a_{1}&\vec a_{2}&\cdots&\vec a_{n}\end{bmatrix}\begin{bmatrix}x_1 \\ x_2 \\ \vdots \\ x_n\end{bmatrix}=x_1\vec a_1+x_2\vec a_2+\cdots+x_n\vec a_n
$$
where
- $\vec{a}_n$ = nth column of the matrix $A$ 

> [!note]
> For this process to work, the vector being multiplied must have the same number of rows as the matrix has columns

>[!note]
>Matrix-Vector multiplication is not commutative. i.e. $A\vec x$ works but $\vec xA$ does not


>[!example]
>$$\begin{bmatrix}2&-3 \\ 8&0 \\ -5&2\end{bmatrix}
\begin{bmatrix}4 \\ 7\end{bmatrix}=\begin{bmatrix}(4)(2)+(7)(-3) \\ (4)(8)+0 \\ (4)(-5)+(7)(2)\end{bmatrix}=\begin{bmatrix}-13 \\ 32 \\ -6\end{bmatrix}$$
