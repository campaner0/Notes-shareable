---
type: note
aliases:
  - Impulse Function
  - Dirac Delta Function
tags: [math, Circuit_Analysis]
---
10/31/2022 20:58

  

The unit impulse function is a "function" that has zero as its output for every input but one ($t_0$), where it is nonzero
$$\delta(t-t_0)
\begin{cases}
=0,\;t\ne t_0 \\
\in\mathbb{R},\;t=t_0
\end{cases}$$

### Sifting Property
When the impulse function is multiplied by another function, the integral of the result is the arbitrary function evaluated at $t_0$. This is especially useful for [[Laplace Transform|Laplace Transforms]].
$$
\int_{-\infty}^{\infty}\delta(t-t_0)f(t)dt=f(t_0)
$$