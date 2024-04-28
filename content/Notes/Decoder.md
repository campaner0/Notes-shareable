---
type: note
tags: [Digital_Logic]
---
09/19/2022 17:18

  

Decoding is the conversion of an $n$ bit code to a $m$ bit output code such that each input code produces a unique output. An $n$-bit input code can represent up to $2^n$ outputs 
$$
n\le m\le 2^n
$$


### Examples
1x2 line decoder
$$\begin{array}{c|c|c}
A&D_0&D_1\\
\hline
0&1&0\\
1&0&1
\end{array}$$
![[1x2 Decoder.png]]


2x4 line decoder 
$$\begin{array}{c|c|c|c|c|c}
A_0&A_1&D_0&D_1&D_2&D_3\\
\hline
0&0&1&0&0&0\\
0&1&0&1&0&0\\
1&0&0&0&1&0\\
1&1&0&0&0&1
\end{array}
$$

![[2x4 Decoder.png]]