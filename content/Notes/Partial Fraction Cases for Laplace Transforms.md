---
type: note
---
11/02/2022 16:35

  #Circuit_Analysis 

When solving differential equations using [[Laplace Transform|Laplace Transforms]] during circuit analysis, when returning to the time domain, the equation may not be in one of the forms on the table. It may be converted into one of these forms if it is in one of the following forms:


### Distinct and Real Poles with no repetition

After factoring, the function is in the following form with its [[Partial Fraction Decomposition]] shown:
$$\begin{align*}
V(s)&=\frac{(s+z_1)(s+z_2)\cdots(s+z_{n-1})}{(s+p_1)(s+p_2)\cdots(s+p_n)}\\
&=\frac{k_1}{s+p_1}+ \frac{k_2}{s+p_2}+\cdots+ \frac{k_n}{s+p_n}
\end{align*}$$
In this case:
$$
k_n=(s+p_n)\cdot V(s)\mid_{s=-p_n}
$$
where
- $s$ = [[Complex Frequency]]
- $z_n$ = zeros
- $p$ = [[Pole]]
- $k$ = constant

After the $k$'s are known, it is simple to take the Laplace transform

---

### Distinct but Complex Poles

If, after factoring and partial fractions:
$$
V(s)= \frac{k_1}{s+\alpha-j\beta}+ \frac{k_2}{s+\alpha+j\beta}
$$
then:
$$
\mathscr{L}^{-1}\{V(s)\}=2|k_1|e^{-\alpha t}\cos(\beta t+\theta_k)u(t)
$$
where
- $\theta_k$ = [[Angle]] of $k$ when in polar form

>[!note]
>$k$ can be found the same way as with real poles, but it will be complex

---

### Repeated Poles

If the function is in the form:
$$\begin{align*}
V(s)&= \frac{N(s)}{(s-p)^2}\\
&= \frac{a_n}{(s+p)^n}+\frac{a_{n-1}}{(s+p)^{n-1}}+\cdots+\frac{a_1}{s+p}
\end{align*}$$
then:
$$
a_{n-k}= \frac{1}{k!} \frac{d^k}{ds^k} \left[(s-p)^nV(s)\mid_{s=p}\right]
$$

---

### Complex Quadratic Factors
If:
$$
V(s)= \frac{N(s)}{(s-p_1)(s-p_2)\cdots(s-p_n)(s^{2}+bs+c)}
$$
then:
$$
v(t)=[k_1e^{p_1t}+k_2e^{p_2t}+\cdots+k_ne^{p_nt}+Me^{\alpha t}\sin(\omega t+\theta)]u(t)
$$
where
$$
M\angle\theta= \left.\frac{(s^{2}+bs+c)V(s)}{\omega}\right|_{s=\alpha+\omega t}
$$
