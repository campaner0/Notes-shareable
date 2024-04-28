---
type: note
---
09/07/2022 17:39

Tags: #Digital_Logic 

The consensus theorem is a [[Boolean Algebra]] theorem that states:
$$
XY+\bar{X}Z+YZ=XY+\bar{X}Z
$$

>[!abstract] Proof
>$$\begin{align*}
XY+\bar{X}Z+YZ&=XY+\bar{X}Z+(X+\bar{X})YZ\\
&=XY+\bar{X}Z+XYZ+\bar{X}YZ\\
&=(XY+XYZ)+(\bar{X}Z+\bar{X}YZ)\\
&=XY(1+Z)+\bar{X}Z(1+Y)\\
&=XY+\bar{X}Z
\end{align*}$$

The dual of this theorem is also true: [[Dual of the Consensus Theorem]]