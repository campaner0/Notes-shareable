---
type: note
tags: [Math]
---
12/14/2022 17:42

  

Matrix operations are opertions involving two [[Matrix|Matrices]] or a scalar and a matrix.

### Addition
The sum of two matrices is calculated by adding the entries of each:
$$
A+B=\begin{bmatrix}a&b&c \\ d&e&f\end{bmatrix}+\begin{bmatrix}g&h&i \\ j&k&l\end{bmatrix}=\begin{bmatrix}a+g&b+h&c+i \\ d+j&e+k&f+l\end{bmatrix}
$$

---

### Multiplication
A matrix may be multiplied by a scalar or another matrix:

#### Scalar Multiplication
If $c$ is a scalar and $D$ is a matrix, $cD$ is calculated by multiplying each element of the matrix by $c$:
$$
cD=c\begin{bmatrix}u&v&w \\ x&y&z\end{bmatrix}=\begin{bmatrix}cu&cv&cw \\ cx&cy&cz\end{bmatrix}
$$


---

#### Matrix Multiplication
Two matricies $A$ and $B$ may be multiplied if $A$ has the same number of rows as $B$ has columns and $A$ has the same number of columns as $B$ has rows. Each entry of the product matrix is calculated as the [[Dot Product]] of a row vector from one matrix and column vector of the other. This operation is not commutative, that is, $AB\ne BA$.
$$
AB=\begin{bmatrix}a&b&c \\ d&e&f\end{bmatrix}\begin{bmatrix}g&h \\ i&j \\ k&l\end{bmatrix}=\begin{bmatrix}ag+bi+ck&ah+bj+cl \\ dg+ei+fk&dh+ej+fl\end{bmatrix}
$$

>[!note]
>[[Matrix-Vector Multiplication]] is a form of matrix multiplication where one matrix has only one column, a [[Vector]]

---

### Transposition
The transpose $A^T$ of a matrix $A$ is found by switching the rows and columns of the matrix. The diagonal remains the same:
$$
\begin{align*}
A&= \begin{bmatrix}a&b&c \\ d&e&f\end{bmatrix}\\[5pt]
A^T&= \begin{bmatrix}a&d \\ b&e \\ c&f\end{bmatrix}
\end{align*}
$$