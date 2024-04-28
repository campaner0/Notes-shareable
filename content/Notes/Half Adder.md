---
type: note
tags: [Digital_Logic]
---
09/21/2022 17:12

  

A half adder adds the bits of a two bit [[Binary]] number 

![[Half-Adder.png]]

|X|Y|Carry|Sum|
|-----|-----|-----|------|
|0|0|0|0|
|0|1|0|1|
|1|0|0|1|
|1|1|1|0|
$$\begin{align}S&=X\oplus  Y \\
&=\bar{X}Y+X\bar{Y}
\end{align}$$
$$
C=XY
$$

This truth table for the sum is similar to an XOR gate's, and the carry is an AND
gate. (see [[Logical Operators]])
