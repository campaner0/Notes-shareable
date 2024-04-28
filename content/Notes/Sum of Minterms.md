---
type: note
---
09/07/2022 18:05

  #Digital_Logic 

A sum of minterms is a shorthand way to write a [[Boolean Algebra]] function. If each variable and its inverse are taken as 1's and 0's, then the function can be written as a sum of [[Binary]] numbers:
$$\begin{align*}
F&=\bar{X}\bar{Y}\bar{Z}+\bar{X}Y\bar{Z}+X\bar{Y}Z+XYZ\\
&=m_0+m_2+m_5+m_7\\
&=(000)+(010)+(101)+(111)\\
&=\sum(0,2,5,7)
\end{align*}$$
