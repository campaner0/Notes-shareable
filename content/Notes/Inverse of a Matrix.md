---
type: note
---
11/16/2022 12:25

  #math 

If $A$ is a square ($n\times n$) [[Matrix]] and there exists a matrix $B$ such that 
$$
AB=I_{n\times n}
$$
where
- $I$ = [[Identity Matrix]]
- $B=A^{-1}$ = inverse of $A$

then the matrix is invertible. If this equation is not true, then the matrix is singular (not invertible).

>[!note]
>A matrix is invertible if is satisfies any of the equivalent statements of the [[Invertible Matrix Theorem]]

---

### Theorems
1. If $A$ is invertible, then $A^{-1}$ is invertible and $(A^{-1})^{-1}=A$ 
2. If $A$ and $B$ are $n\times n$ and invertible, $AB$ is invertible and $(AB)^{-1}=B^{-1}A^{-1}$
3. Any sequence of [[Elementary Row Operations]] that reduce $A$ to $I$ also reduces $I$ to $A^{-1}$

---

### 2x2 Matrix Inversion
There is a formula for the inverse of a 2x2 matrix:
$$\forall A=
\begin{bmatrix}a&b \\ c&d\end{bmatrix},\;\;\; A^{-1}= \frac{1}{ad-bc}
\begin{bmatrix}d&-b \\ -c&a\end{bmatrix}$$
where
- $\frac{1}{ad-bc}$ = [[Determinant]] of $A$

For larger matrices, theorem 3 above must be used to find the inverse.