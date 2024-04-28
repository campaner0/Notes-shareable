---
type: note
alias: Euler's Identity
tags: [math]
---
01/23/2023 13:32

  

Euler's Formula relates the trigonometric functions to the complex exponential function:
$$
e^{\pm ix}=\cos(x)\pm i\sin(x)
$$
where 
- $x\in\mathbb{R}$ 

Euler's Identity is revealed when $x=\pi$:
$$
e^{i\pi}=-1
$$

## Proofs
This formula can be proven using [[Power Series]]. The power series definition of the complex exponential function is the sum of the power series of sine and cosine:
$$\begin{align*}
e^{ix}&=\sum\limits_{n=0}^{\infty}\frac{(ix)^n}{n!}\\[5pt]
&= \sum\limits_{n=0}^{\infty}\frac{(-1)^nx^{2n}}{(2n)!}+i\sum\limits_{n=0}^{\infty}\frac{(-1)^nx^{2n+1}}{(2n+1)!}\\[5pt]
&= \cos(x)+i\sin(x)
\end{align*}$$

