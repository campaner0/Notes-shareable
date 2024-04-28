---
type: note
tags: [math]
---
11/17/2022 18:22

  

The determinant of a square [[Matrix]] $A$ is a scalar value derived from the elements of the matrix. If the determinant of $A$ is nonzero, $A$ is invertible according to the [[Invertible Matrix Theorem]]. 

### 2x2 Matrix
The determinant for a matrix $A=\begin{bmatrix}a&b\\c&d\end{bmatrix}$ is given by:
$$
|A|=\left|\begin{matrix}a&b\\c&d\end{matrix}\right|=ad-bc
$$

---

### 3x3 Matrix
For a 3x3 matrix:
$$|A|=\begin{align*}
\left|\begin{matrix}a&b&c\\d&e&f\\g&h&i\end{matrix}\right|&=a\left|\begin{matrix}e&f\\h&i\end{matrix}\right|-b\left|\begin{matrix}d&f\\g&i\end{matrix}\right|+c\left|\begin{matrix}d&e\\g&h\end{matrix}\right|\\
&= a(ei-fh)-b(di-fg)+c(dh-eg)
\end{align*}$$
The shown formula is only one of many ways to arrange the variables. Instead of starting with the top row, one may use the first column. This would change the 2x2 matrices as well since they are made up of the elements not in the starting row/column or the row/column of the current variable.