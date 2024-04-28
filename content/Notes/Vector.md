---
type: note
---
03/25/2022 18:20

Tags: #math, #Physics, #Statics, #Electromagnetics, #Linear_Algebra 

A vector is a mathematical concept that has both [[Magnitude]] and direction, and is often denoted with an arrow above a letter or a bold letter e.g. $\vec v$ or $\mathbf v$. 

### Notation
Vectors may be written with their elements between angled brackets or using the standard [[Unit Vector|Unit Vectors]]:
$$\vec{v}=\begin{cases}
\langle v_1,\,v_2\,\cdots,\,v_n\rangle \\[5pt]
v_1\hat{x}+v_2\hat{y}+v_3\hat z
\end{cases}$$

#### Linear Algebra
In linear algeba, a vector is denoted as a [[Matrix]] with one column (column vector):
$$
\vec{v}=\begin{bmatrix}v_1 \\ v_2 \\ \vdots \\ v_n\end{bmatrix}
$$
or a matrix with one row (row vector):
$$
\vec{u}=\begin{bmatrix}u_1&u_2&\cdots&u_n\end{bmatrix}
$$

---

### Operations
Vectors may be operated on similarly to scalars with addition and (some) multiplication

#### Addition
The sum of two vectors is a vector whose elements are the sums of the two vectors' elements:
$$
\vec{v}+\vec{u}=\langle v_1+u_1,\,v_2+u_2,\,\cdots,\,v_n+u_n\rangle
$$

---

#### Multiplication
To multiply a vector by a scalar, simply multiply the each of the elements of the vector by the scalar:
$$
c\vec{v}=\langle cv_1,\,cv_2,\,\cdots,\,cv_n\rangle
$$
where
- $c$ = scalar value

>[!note]
>Two or more vectors cannot be multiplied by simply multiplying the elements like scalar multiplication. Multiplication with vectors is defined in several ways:
[[Dot Product]], [[Cross Product]], [[Triple Product]]
