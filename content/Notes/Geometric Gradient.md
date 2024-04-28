---
type: note
---
08/30/2023 13:03

  #engineering_econ 

A geometric gradient changes cash flow by a certain percentage each year, as opposed to an [[Arithmetic Gradient]] which changes by a fixed amount. The ratios of consecutive terms are equal.

To find [[Current Value|P]] for a geometric gradient:
$$\begin{align*}
P_{g}&= A_1(P/A_{1},g,i,n)\\[5pt]
&= \begin{cases}
A_1\left[\frac{1-\left(\frac{1+g}{1+i}\right)^{n}}{1-g}\right],\text{if}\,g\ne i\\[5pt]
A_{1}\left(\frac{n}{1+i}\right)\qquad\,\,,\text{if}\,g=i
\end{cases}
\end{align*}$$
where
- $P_g$ = present worth with gradient
- $A_1$ = cash flow at first period
- $g$ = rate of increase
- $i$ = [[Interest and Interest Rate|Interest]]
- $n$ = number of [[Time]] periods
